# ConwaysGameOfLife
Authors: NachoCainelli(https://github.com/NachoCainelli) and joaquinarroyo(me)

Conway's game of life implemented with threads in C

The Game of Life was posed by the mathematician John Horton Congway in 1970. It's a game without players who posed as a cellular automaton. This means that the only interaction is given at the beginning of the game, posing a board initial, and then the system will evolve following the established rules.

At each moment, the cells become alive or dead following the rules:

- Every living cell with 2 or 3 living neighbors survives,
- Every dead cell with exactly 3 living neighbors revives,
- The rest of the living cells die in the next generation, as in turn
- the rest of the dead cells remain dead.

We then assume that the borders are shared, folding the board. That is, the upper border is the lower border, while theleft border is the right border.

The reading of the game will be given in a file respecting the following format:

on a line 3 positive integers indicating the number of cycles (C), the number of rows (M) and the number of columns (N) that the board will have, then the board described in format RLE, taking the values 'X' or 'O', representing dead and living cells respectively.

for example:

10 3 3

3X

3O

3X

This input will lead us to a simulation where the cycles are 10, the board is 3x3 and it is like this:

XXX

OOO

XXX

To compile the program you can use the next command 
```
make simulador
```

The compilation of the solution should leave an executable in the directory of name 'simulador'. And the executable is expected to take as standar input the name of the file where the board is. 
For example 
```
./simulador "board.txt"
```

You've a report in spanish. (Working on a report in english 💤)

