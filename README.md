# Sudoku Solver

This Python program solves Sudoku puzzles using a backtracking algorithm. It provides a textual representation of the Sudoku board and can solve standard 9x9 puzzles.

## Features

- Solve standard 9x9 Sudoku puzzles.
- Support for custom puzzle sizes that fit the 9x9 square format.
- Display a stylized ASCII representation of the Sudoku board.
- Utilize a backtracking algorithm to efficiently solve Sudoku puzzles.
- Check constraints (rows, columns, and 3x3 subgrids) to ensure valid moves.

## Implementation Details

The solver uses a recursive backtracking algorithm to explore possible solutions for the Sudoku puzzle. It follows these steps:

1. **Finding an Empty Cell**: Locate the next empty cell (cell with value `0`) on the Sudoku board.
2. **Validating Potential Numbers**: For each empty cell, attempt to place numbers `1` to `9` that satisfy Sudoku rules (no repeated numbers in rows, columns, or 3x3 subgrids).
3. **Backtracking**: If a number doesn't lead to a valid solution, backtrack by resetting the cell's value and trying the next potential number.

The solver recursively applies these steps until a valid solution is found or determines that the puzzle is unsolvable.
