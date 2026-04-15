# Sudoku-Boards-as-CSPs

This repository contains a Sudoku CSP solver for the assignment question on backtracking search, forward checking, and AC-3.

## Contents

- [23F-0550.ipynb](23F-0550.ipynb): the main notebook with the CSP solver and report output
- [easy.txt](easy.txt), [medium.txt](medium.txt), [hard.txt](hard.txt), [veryhard.txt](veryhard.txt): the four Sudoku boards
- [sudoku_results.txt](sudoku_results.txt): saved solver output with solved boards and BACKTRACK statistics

## What the solver does

The notebook implements a CSP-based Sudoku solver using:

- backtracking search
- forward checking
- AC-3 arc consistency
- MRV and degree heuristics for variable selection

## Input format

Each board file must contain exactly 9 lines, and each line must contain exactly 9 digits.

- `0` means an empty cell
- digits `1` to `9` are fixed clues

## How to run

Open [23F-0550.ipynb](23F-0550.ipynb) and run the cells from top to bottom. The notebook reads the four `.txt` files, solves them, and prints the results and statistics.

If you want to regenerate the saved report file, run the notebook to completion and copy the printed output into [sudoku_results.txt](sudoku_results.txt).
