---
title: 'The Game of Life'
date: 2024-10-08T20:08:38+05:30
draft: false
tags: [programming, mathematics, cellular automata, computing]
---
|![conway](https://github.com/ShirakuGIT/mathemagic/blob/main/conway/conway_sim.gif?raw=true "Conway's Game of Life")|
|:--:|
|[*Rendering of Conway's Game of Life*](https://github.com/ShirakuGIT/mathemagic)|

# Table of Contents
1. [Cellular Automata](#cellular-automata)
2. [Conway's game of life](#conways-game-of-life)
3. [Rules](#rules)
4. [Implementation](#implementation)
5. [Shortcomings](#shortcomings)

## Cellular Automata

Cellular Automata is a field of computer science dealing with modelling certain systems by dividng a space into a grid of cells, each cell can take upon a finite number of states.
The states are then influenced and modified according to a set of rules which similarly influence neighbouring cells.

Very simply put, its a box of cells, that can take a state and are influenced / can influence their neighbours based on a set of rules. 

## Conway's game of life

[The game of life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life#) is a [cellular automaton](https://en.wikipedia.org/wiki/Cellular_automaton) invented by *John Horton Conway* in 1970. It's most famously known as a **zero player game**. It's a fancy way of saying that the game's progression depends on an initial state, and that's it, no other factors / players / events influence it a.k.a **automata**.

## Rules

The Rules are simple:
- Any live cell with fewer than two live neighbours dies (underpopulation).
- Any live cell with more than three live neighbours dies (overcrowding).
- Any dead cell with exactly three live neighbours becomes a live cell (reproduction).
- Any other state remains unchanged (stasis).

## Implementation

Very roughly the pseudocode can be written as so:
```pseudocode
Initialization:

    Set up a 2D grid with alive or dead cells.
    Start with an initial pattern.

Main Loop:

    For each cell:
        Count neighbors.
        Apply rules:
            Dies (under/overpopulation).
            Becomes alive (reproduction).
            Stays alive (survival).
        Record changes.

    Apply changes and redraw changed cells.

    Repeat until stopped or stable.
```
I have written the C++ code with a graphics library implementation using SFML [here](https://github.com/ShirakuGIT/mathemagic/blob/main/conway/conway.cpp). Also, if you're already visiting, kindly make sure to check out my other projects within the same [repository](https://github.com/ShirakuGIT/mathemagic)! Thanks.

## Shortcomings

The code works, but there’s room for improvement. First, use **double buffering** to avoid in-place updates affecting neighboring cells during the same generation. Second, optimize **neighbor calculation**—it’s repetitive and slow for larger grids. Precomputing or caching neighbor positions would help. Third, **preallocate the `generation` vector** to avoid frequent resizing, which slows things down. Lastly, avoid creating new rectangles on every frame; instead, store them and just update colors. These changes would significantly improve both correctness and performance.