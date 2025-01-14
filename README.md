# This Python program solves a 9x9 Sudoku puzzle using the backtracking algorithm. Given an incomplete Sudoku grid, the program attempts to fill in the empty cells with digits from 1 to 9 such that each row, column, and 3x3 sub-grid contains all digits from 1 to 9 without repetition.


## Features
- Solves a 9x9 Sudoku puzzle using the backtracking algorithm.
- Takes a 9x9 grid as input, where empty cells are rapresented by `0`.
- Modifies the input grid in place to fill in the correct numbers.
- Returns `True` if a solution in found, and `False` if no solution exists.


## Example Usage

Here is an example of how to use the Sudoku solver solver with a sampe puzzle:

```Python
board = [
    [5, 3, 0, 0, 7, 0, 0, 0, 0],
    [6, 0, 0, 1, 9, 0, 0, 0, 0],
    [0, 9, 8, 0, 0, 0, 0, 6, 0],
    [8, 0, 0, 0, 6, 0, 0, 0, 3],
    [4, 0, 0, 8, 0, 3, 0, 0, 1],
    [7, 0, 0, 0, 2, 0, 0, 0, 6],
    [0, 6, 0, 0, 0, 0, 2, 8, 0],
    [0, 0, 0, 4, 1, 9, 0, 0, 5],
    [0, 0, 0, 0, 8, 0, 0, 7, 9]
]
