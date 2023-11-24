# Hog-project-CIS61
Introduction

In this project, you will develop a simulator and multiple strategies for the dice game Hog. The goal is to use control and higher-order functions from Sections 1.1 through 1.6 of the Composing Programs online text.

Game Overview
In Hog, two players alternate turns trying to reach 100 points first. Players choose the number of dice to roll on their turn, and the turn score is the sum of the dice outcomes, with special rules like Pig Out, Free Bacon, Hog Wild, and Swine Swap.

Project Files
This project includes six files, but all changes will be made to the first one, hog.py. The other files are provided for utility and testing purposes.

hog.py: Starter implementation of Hog.
dice.py: Functions for rolling dice.
ucb.py: Utility functions for CS 61A.
hog_gui.py: A graphical user interface for Hog.
hog_grader.py: Tests to check the correctness of your implementation.
autograder.py: Utility functions for grading.
Logistics

This is a multi-week project and not a group project.
Start early, as the time required for completion can be unpredictable.
The project is worth 10 points, with 9 points assigned for correctness and 1 point for the overall composition of your program.
You are only required to work on hog.py. Do not modify other files or function signatures.
Graphical User Interface
A GUI is provided for you. After finishing Problem 4, you can play a fully interactive version of Hog. Make sure Tkinter is installed, then run the GUI from your terminal:

bash
Copy code
python3 hog_gui.py
Testing

Throughout the project, test the correctness of your code. Run tests often to isolate any problems. Tests are contained in docstrings and hog_grader.py.

To run all tests:

bash
Copy code
python3 hog_grader.py
Run tests for a specific question:

bash
Copy code
python3 hog_grader.py -q 1
Additionally, you can call certain functions interactively from the terminal:

bash
Copy code
python3 hog.py -i roll_dice
Phase 1: Simulator

In this phase, you will develop a simulator for the game of Hog. Follow the instructions in the project description to complete Problems 1 to 4 in hog.py.

Problem 1 (1 pt): roll_dice
Implement the roll_dice function.

Problem 2 (1 pt): take_turn
Implement the take_turn function.

Problem 3 (1 pt): select_dice
Implement the select_dice helper function.

Problem 4 (2 pt): play
Implement the play function to simulate a full game of Hog.

Phase 2: Strategies

In the second phase, you will experiment with ways to improve upon the basic strategy of always rolling a fixed number of dice. Follow the instructions to complete Problems 5 to 9 in hog.py.

Problem 5 (1 pt): make_averaged
Implement the make_averaged function.

Problem 6 (1 pt): max_scoring_num_rolls
Implement the max_scoring_num_rolls function.

Problem 7 (1 pt): bacon_strategy
Implement the bacon_strategy function.

Problem 8 (1 pt): swap_strategy
Implement the swap_strategy function.

Problem 9 (1 pt): final_strategy
Implement the final_strategy function by combining strategies to achieve a win rate of at least 0.59 against the baseline strategy.

Running Experiments
Change the implementation of run_experiments as needed and use average_win_rate to evaluate various Hog strategies.

Play Against Your Strategy
Use the graphical user interface to play against your final strategy:

bash
Copy code
python3 hog_gui.py -f
