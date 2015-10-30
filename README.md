# Summary

This project is a solver for the 0hh1.com version of the Tazuku puzzle. It is written using Python.

# Table of Contents

* [The Solvers](#solvers)
* [Requirements](#reqs)
* [How to Use](#how-to)
* [Future Improvements/Expansions](#future-features)
* [Credit](#credit)

# <a name="solvers"></a>The Solvers
There are two solvers included.
The 0hh1.py solver solves the puzzle entirely then outputs the solution by clicking on the board.
The 0hh1v.py solver clicks the board each time it makes a move, showing how the solver is attempting the problem.

# <a name="reqs"></a>Requirements

This app was written entirely with Python. It requires Python2.
The following libraries need to be imported: PIL (pillow), win32gui, win32api, win32con

# <a name="how-to"></a>How to Use
The program can be run using the command 'python [solver-file]'. It will give you prompts, which say:
* Position your cursor at the top-left corner of the board and press enter.
* Position your cursor at the bottom-right corner of the board and press enter.
* Board dimension:

The board dimension is the width or height of the board (which should be equal).
After inputting the board dimension, leave the mouse cursor alone as it will be moved around to solve the puzzle.

# <a name="future-features"></a>Future Improvements/Expansions

There are some more optimizations that can be added to the solver, such as not checking every single cell and instead maintaining a list of cells that need to be checked. It might be possible to also add a smarter guessing algorithm, as it currently just goes through cells in order, and stores potentially useless information (due to pruning).

The app also needs to check that the board itself is valid earlier. If I can figure out how to recognize the original non-user cells, then it would be possible to have the algorithm fix the table into a valid solution.

Eventually it would be nice to have the program detect the board without needing user input, perhaps using the OpenCV library.

Another possibility would be to look into the source code and see if its possible to pull the board state directly from the website.

Or even create a similar website with the solver built in, and allow for users to create their own boards (which may or may not have solutions).

# <a name="credit"></a>Credit
Written by Andrew Zhao (2015)