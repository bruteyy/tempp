# Practical 1: Basic Graphics Primitives

## Problem Statement
Implement and display basic Graphics primitives such as points, lines, and polygons.

## Aim
To draw a line on the screen using the graphics primitives of `graphics.h` in Turbo C.

## Theory
A graphics primitive is a basic shape from which bigger drawings are built. `graphics.h` provides ready functions for them:

| Primitive | Function |
|-----------|----------|
| Point | `putpixel(x, y, color)` |
| Line | `line(x1, y1, x2, y2)` |
| Polygon | `drawpoly(n, points)` |

## Algorithm
1. Include `graphics.h` and `conio.h`.
2. Declare `gd = DETECT` so the graphics driver is detected automatically.
3. Call `initgraph()` with the path of the BGI folder to start graphics mode.
4. Draw the line from (100, 150) to (400, 150) using `line()`.
5. Wait for a key press using `getch()`.
6. Call `closegraph()` to return to text mode.

## Requirements
- Language: C / C++
- Compiler: Turbo C++ (with BGI folder at `C:\TURBOC3\BGI`)

## How to Run
Open `main.cpp` in Turbo C++, press `Alt + F9` to compile and `Ctrl + F9` to run.

## Output
![Output](output.png)

## Viva Questions
1. **What is `initgraph()`?** It switches the screen to graphics mode and loads the graphics driver.
2. **What does `DETECT` do?** It makes the system detect the graphics card and pick the best driver and mode automatically.
3. **What is the BGI path?** The folder that holds the Borland Graphics Interface driver files (`.bgi`), needed by `initgraph()`.
4. **Why is `getch()` used?** It holds the output screen until a key is pressed, otherwise the window closes instantly.
5. **What does `closegraph()` do?** It closes graphics mode and frees the memory used by the graphics system.
6. **What are the arguments of `line()`?** `line(x1, y1, x2, y2)`: start point and end point.
