# Algorithm Visualizer

An interactive web application that animates how classic algorithms work step by step, helping users build intuition for concepts that are usually only seen as static pseudocode.

## Overview

Algorithm Visualizer turns abstract algorithms into real-time, animated visuals. Users can generate random data, tweak inputs, control playback speed, and watch each comparison, swap, or traversal happen live — turning "how does quicksort work?" into something you can *see* instead of just read.

## Algorithms Covered

**Sorting**
- Bubble Sort, Selection Sort, Insertion Sort
- Merge Sort, Quick Sort, Heap Sort
- Counting Sort, Radix Sort

**Searching**
- Linear Search, Binary Search

**Graph Algorithms**
- BFS, DFS
- Dijkstra's Shortest Path
- A* Pathfinding
- Minimum Spanning Tree (Prim's / Kruskal's)

**Pathfinding / Grid-based**
- Maze generation and solving
- Obstacle-based pathfinding visualizer

**Trees**
- Binary Search Tree insert/delete/traverse
- AVL / Red-Black tree rotations (optional stretch goal)


## Project Structure (suggested)

```
AlgorithmVisualizer/
├── src/
│   ├── sorting/
│   ├── searching/
│   ├── graph/
│   └── pathfinding/
└─── README.md
```

## How It Works

1. The algorithm logic is instrumented to emit a sequence of "steps" (e.g., `{ type: 'compare', indices: [i, j] }`) instead of just returning a result.
2. Steps are queued and played back on a timer, updating the visual state (colors, positions) frame by frame.
3. The UI subscribes to the current step to drive highlighting, stats, and pseudocode-line tracking.

## Possible Enhancements

- Dark mode / theme switcher
- Shareable permalink with algorithm + input state encoded in the URL
- Sound effects tied to comparisons/swaps
- Mobile touch controls for grid-based pathfinding
- Algorithm race mode (compare two algorithms side by side on the same data)

---

Feel free to trim this down or expand specific sections (e.g., add screenshots/GIFs, a live demo link, and installation instructions) once the implementation is further along.
