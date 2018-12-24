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
