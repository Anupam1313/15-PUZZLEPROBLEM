Given a 4×4 board with 15 tiles (every tile has one number from 1 to 15) and one empty space. The objective is to place the numbers on tiles in order using the empty space. We can slide four adjacent (left, right, above and below) tiles into the empty space.

In general, for a given grid of width N, we can find out check if a N*N – 1 puzzle is solvable or not by following below simple rules : 
 

1. If N is odd, then puzzle instance is solvable if number of inversions is even in the input state.
2. If N is even, puzzle instance is solvable if
   * the blank is on an even row counting from the bottom (second-last, fourth-last, etc.) and number of inversions is odd.
   * the blank is on an odd row counting from the bottom (last, third-last, fifth-last, etc.) and number of inversions is even.
3. For all other cases, the puzzle instance is not solvable.
