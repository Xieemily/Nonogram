# Nonogram
A nonogram generater and solver， generate hint from image or solve game provided hint, all possible solutions can be found.（ongoing）



## How To Run

**User interface is not added yet, so run it from command line with options below:**

`-s` 		solve mode, enter board size `n` and hint (n*n square board)

`-g` 		generate mode, enter image path



## Usage

- ### Generate game from image:

  <img src="./media/einstein.jpg" style="zoom:26%;" />        <img src="./media/einstein_game2.jpg" style="zoom:40%;" />

  hint will be printed.

- ### Solve game given hint

Board size: 2     (2*2)

Row hint: 

1 1

1 1

Col hint:

1 1

1 1

Solved:

**solution1:** 0101101001011010
⬜⬛⬜⬛
⬛⬜⬛⬜
⬜⬛⬜⬛
⬛⬜⬛⬜
**solution2:** 1010010110100101
⬛⬜⬛⬜
⬜⬛⬜⬛
⬛⬜⬛⬜
⬜⬛⬜⬛



For game with more than 50 solutions, only the first 50 solutions will be generated, this number can be changed by setting `SULUTION_NEED` to the amount you need.



Game of size 100*100 can be solved within 1 second (per solution), as for solving the hint generated from the Einstein picture above, 50 solutions can be found in about 12 seconds (0.2 s per solution).