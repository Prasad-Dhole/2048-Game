# 2048-Game

About Game --> 
    You will have a 4 X 4 Matrix, in which two randomly selected cells will have ‘2’ as their value.
    Use the arrow keys to move all cells in the corresponding direction
    While cells move in a particular direction same values will add up to combine into a single cell and different value cells will simply move in that particular direction if there are empty cells
    The magnitude of the value assigned will increase as the game moves on. Also, empty cells will randomly be assigned with random values. All values will be of some power of 2.
    You have to smartly make combinations such that you reach the number 2048. This is the winning condition.


Approach --> 
First, create a 4 X 4 matrix using a CSS grid. Each cell is an HTML div tag with a p tag inside to hold its text.
Define a function in Javascript to randomly pick a cell and assign it a value
Use JavaScript event listeners in moveBlocks to acknowledge the key press events like arrow keys and to shit cells in that corresponding direction directed by the arrows.
Assign different colors to the cell containing different values and also to the empty cell.
Create function shift(direction) and move(direction) to shift the values in case of empty cells and combine the same values respectively
Check the max value in the cells and use the gameOver function to show winning dialogue if the max value reaches 2048 and losing dialogue in case of no cells in empty and the max cell value has not reached 2048.