# Lab 6 - javascript

*Use the lecture notes to recall the main JavaScript concepts from [lecture 6](https://cs.unibuc.ro/~cechirita/twe/c6) and solve the following exercises.*  

## I'm a cyborg, but that's OK. 

1. Play the first 6 levels of the game [jsrobot](https://tantemalkah.at/jsrobot/) to quickly review some javascript basics.
 
## tic-tac-toe

*Solve the exercises below to implement a tic-tac-toe game with an ASCII interface using JavaScript.   
Create an html file `ttt.html` with an empty `body` element, in which you should include a JavaScript file `ttt.js`. Solve the exercises by editing the file `ttt.js`.*

2. Using `prompt`, display the message *"Let's play tic-tac-toe. What's your name?"* and save the user's reply in a variable.

3. Display the message *"Hello, < name >. Who do you want to be? X or 0? X starts first."* and save the answer in a variable. 

4. Use an `Array` to represent the grid game. The `Array` consist of 9  `Strings`: the first 3 elements represent the first line of the grid, the next 3 the second line, and the last 3, the third line. Initialize each element with `String` *"?"*, indicating the fact that all the 9 cells are empty.  
*Hint: use a `for` instruction.*

5. Write a function `printtt` which returns an ASCII representation of the grid. For example, for the grid `["?", "?", "X", "?", "0", "?", "?", "?", "?"]`, it could return    
`| 1 | 2 | X |`  
`| 4 | 0 | 6 |`  
`| 7 | 8 | 9 |`.  
In the representation above, in each cell we write `X` if the `Array` contains the string `"X"` at that position, `0` if it contains the string `"0"`, or its position, if the cell is empty (meaning that the `Array` contains `"?"` at that position).    

6. We start playing Xs and Os alone, without an adversary. Using `prompt`, display the grid and the message *"Where do you want to place the next sign?"*. Save in a variable the grid position. 

7. Write a function `valid` that checks if the position entered by the player is valid: if it is a position on the grid (a number between 1 and 9) and if the cell at that position is empty. The function should return a `boolean` value. 

8. If the position entered by the player is not valid, you must display a warning message and repeat step 6. If the position is valid, add the player's sign in the grid and repeat step 6.

Our game runs for now in a loop, without ending. Even if the grid is full, the user will be prompted with a request for the next position at which they want to add a sign.

9.  Write a function `win` that checks if the grid is in a winning configuration (if there are 3 X or 0 symbols on the same row, column, or diagonal) and that returns the winning symbol. 

10. Write a function `draw` that checks if the grid is in a draw configuration, returning a `boolean`. 

11. Change the code of the game to check, after each turn of the player, what is the state of the game and display (using `alert`):
- the message *"Congratulations, < name >, you won!"*, if the player has won, 
- the message *"You lost :("* if the player has lost, or 
- the message *"Draw!"* in case of a draw.
Continue the game otherwise.

12. It's time to invite an opponent to our game: the computer. Write a function `computer_move` that generates randomly, using `Math.random()`, a grid position corresponding to the next position to be played by the computer. Check if the position is valid using the function `valid` from exercise 7. If the position is valid, fill in the grid accordingly. Otherwise, call again the function `computer_move`. 

13. Plug in the code for the exercise above such that the player and the computer each make a move alternatively, and the game finishes when a winning or draw configuration is reached. 

14. Bonanza extravaganza! Let's play two tic-tac-toe games in parallel!  
Rewrite the code such that the player can play against the computer two different games in parallel. In this way, in each `prompt` we will display two grids, and the player will enter two  positions (separated by a blank space), one for each grid. The player continues to play until both games finish. 

*Hint: To solve this exercise you will have to create objects of type `game` which will contain properties for representing the grid and the player (with corresponding properties for the name and sign chosen) and methods which correspond to the functions that you wrote to solve the exercises above (`printtt`, `valid`, `win`, `draw`, `computer-move` etc.).*        

## EXTRA

15. Play [Untrusted - The Continuing Adventures of Dr. Eval](https://alexnisnevich.github.io/untrusted/).
 

