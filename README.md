# rubiks-cube-solver
This project is a web-based application designed to simulate and solve a standard 3x3 Rubik's Cube. It serves as a demonstration of object-oriented programming, algorithm design, and front-end development skills.

## Features

* **Object-Oriented Cube Representation:** Manages the cube's state and logic using a dedicated class.
* **Manual Rotations:** Supports all 12 standard Rubik's Cube face rotations (U, D, L, R, F, B and their inverses).
* **Cube Scrambling:** Generates random, solvable scrambled states.
* **Step-by-Step Solving Algorithm:**
    * Implements a beginner-friendly, layer-by-layer method.
    * Prioritizes functionality and clarity over finding the mathematically optimal solution.
* **Visual Step-by-Step Display:** Shows the cube's state after each significant solving step with a description.
* **Interactive UI:** Includes buttons for scrambling, solving, resetting, and performing individual manual moves.
* **Clear Visuals:** Uses SVG for a 2D cube representation with a dark background for contrast.

## How to Use

* **Clone or Download:** Get the `rubiks_cube_solver.html` file from this repository.
* **Open in Browser:** Simply open the `rubiks_cube_solver.html` file in any modern web browser.
* **Interact:**
    * Click "Scramble Cube" to randomize.
    * Use face rotation buttons for manual control.
    * Click "Solve Cube" to run the automated solver.
    * Click "Reset Cube" to return to the solved state.

## Technologies Used

* **HTML5:** For page structure.
* **CSS3 (Tailwind CSS):** For styling and responsive layout.
* **JavaScript (Vanilla JS):** For all cube logic, algorithm, and UI interactions.
* **SVG:** For cube rendering.

## Algorithm Overview (Beginner's Method)

The solving algorithm proceeds in a layer-by-layer fashion:

* **White Cross:** Solves the white edge pieces on the bottom face.
* **White Corners:** Inserts the white corner pieces into the bottom layer.
* **Middle Layer:** Places the middle layer edge pieces.
* **Orient Last Layer Edges (Yellow Cross):** Forms a yellow cross on the top face.
* **Permute Last Layer Corners:** Moves top layer corners to their correct positions.
* **Orient Last Layer Corners:** Orients top layer corners so yellow stickers face upwards.
* **Permute Last Layer Edges:** Places top layer edges into their final positions.
