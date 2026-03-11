# Tower of Hanoi Puzzle 
The Tower of Hanoi is a mathematical puzzle where you have three rods and a number of disks of different sizes. <br><br> The objective is to move the entire stack from the source rod to the target rod, following these rules:
1. Only one disk can be moved at a time.
2. Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack.
3. No disk may be placed on top of a smaller disk.

## Project Structure
This project is a part of my learning journey around Python and Algorithms that is based on freeCodeCamp Scientific Computing with Python curriculum. This project has two different solving methods, and I separate it by branches:
* `main` branch: Contains the **Recursive** solution. This is the most common way to solve the puzzle, using a function that calls itself to break the problem into smaller sub-tasks.
* `iterative-hanoi` branch: Contains the **Iterative** solution. This approach uses a loop and mathematical logic (using the modulo operator) to determine the next valid move without recursion.

## How it Works
1. **Recursive Version (main)**
it follows three simple steps:
* Move $n-1$ disks from Source to Auxiliary.
* Move the largest disk from Source to Target.
* Move the $n-1$ disks from Auxiliary to Target.
<br><br>
2. **Iterative Version (iterative branch)**
it calculates the total number of moves required ($2^n - 1$) and uses the move index to decide which disks to swap.

## How to Run
1. Clone the repository.
2. To run the recursive version, stay on the `main` branch and run:
```bash
python hanoi.py
```
3. To check the iterative version, switch branches:
```bash
git checkout iterative-hanoi
python hanoi.py
```
