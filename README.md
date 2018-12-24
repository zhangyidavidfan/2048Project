# 2048Project
CIS 120 Final Project

Game Description: 2048 is a single-player sliding block puzzle game
        		designed by Italian web developer Gabriele Cirulli.
        		The game's objective is to slide numbered tiles on a grid
        		to combine them to create a tile with the number 2048.
        		upon starting you could choose whether or not you would
        		want to read in the saved progress from the last game  
        		CONTROLS: 
        		Use the arrow keys to move the tile
        		Use the save score button to save your score 
        		Use the save progress button to save the game progress
        		Use the leader board button to check the leader board
        		Use the reset button to reset the board
        		NOTE
        		Reading in saved Progress will not read in the scores

Overall implementation: The game starts with the board class that basically
						is a 2d array storing the relevant tile numbers
						it also contains method that could be called on the
						array such as movements, drawing of the tile or checking 
						whether or not any moves are left for the array. This class 
						is then called by the GameCourt file which is where the game
						set up really comes in. This is where a lot of the inputs
						of the users are used to construct the board where the game
						is played. This is also where the multiple method under
						the board class can now interact with each other. This file
						is then used by the Game File, which is where the whole game
						gets pieced together and starts. Here is where all the additional
						buttons are made, and where the location of the game court is
						being specified. Test cases where also used to test the methods
						within the board class.

Concepts implemented: 1. 2d-array - The 4 by 4 2048 board is represented using a 
					  2D array of integers. The state of each non-blank square 
					  will be stored with their corresponding numbers(2, 4, 8 and etc.) 
					  while the blank squares will be given the integer 0. 
					  
					  2. Collection - My 2048 implementation used collections to extract 
					  the three high scores and the user name corresponding to it. Specifically, 
					  the user can prompt to save their score within the duration or after 
					  their game. the scores will be stored in a Maps, that matches the user
					  name to his/her scores. When sorting for the top three scores, the score
					  map’s value will be ordered and displayed.  
					  
					  3. File IO - My 2048 implementation used I/O to store game state. 
					  Specifically, when the save button is pressed, the state of the 2D array 
					  will be saved in a text file. The text file will be accessible whenever 
					  a player wants to load the saved game.
					  
					  4. Test Cases	- I created methods that updates the tiles in all directions.
					  I also have methods that checks the status of the board, and adjacent tiles. 
					  These functionality were tested it with JUnit. Specifically updating of the 
					  2D array is heavily checked. I tested edge cases, such as testing if the 
					  game knows when the game is supposed to end, when a user attempts to move 
					  the tiles when none of it can be moved and when possibility of double collision
					  is possible. 

Classes: There is really only one class that I created and it is the board class I mentioned above
