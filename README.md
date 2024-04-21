# sp24-lab13
Materials for week 13 lab in CS-370, which includes Ch. 24 "Undo and Redo" adapted from [Software Design by Example](https://third-bit.com/sdxpy/) by Greg Wilson.

_April 23, 2024_

Organization:
* SDX-ch24: The code files for the _SDX Ch. 24_ activity, as downloaded from the book website. The test scripts have been modified to include the test runner from chapter 6.

## Team Members for Part 1
Enter your names here

## Team Roles for Part 1
Who will start out as
* DRIVER: Driver's name
* NAVIGATOR: Navigator's name

You will switch halfway through this activity.

## Part 1 Documentation

Write your answers to the questions below.

* What were the main ideas from SDX chapter 24?
* What questions did you have about the material in the chapters? What did you find confusing?

## Exercise 0: Run the code

First, verify that you can run the test scripts, and that all tests pass.

Next, verify that you can run the base application from Chapter 23:

    python3 app.py 20

Use CTRL-X to quit.

Finally, note that Wilson didn't give us a way to run the new code from Chapter 24 as an interactive text editor.
Try running `undoable.py` and verify nothing happens.
We'll address this in a later exercise.

## Exercise n: A real text editor

Create a new main module `main.py`.  It should take the name of a file and open that file for editing using the `UndoableApp` class.

To run the app with a real screen in the terminal, you will need to make the `InsertDeleteApp` class inherit from `App` instead of `HeadlessApp`.
Do this now and resolve any resulting bugs. Note you will no longer be able to run the automated tests that use headless mode.

Then, add a handler for CTRL-S to save the file.

Using your knowledge of design principles and patterns, propose a different approach for introducing headless mode
that would allow you to both use the app and run automated tests.
