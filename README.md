# othello-reinforcement-learning

Play the game of Othello using AlphaZero reinforcement learning algorithm. AlphaZero utlizes a Monte Carlo Tree Search to self learn the best possible move from a given state. The Monte Carlo Tree Search allows for AlphaZero to run simulations from a given state to look ahead and see what the outcome will take place from a given move. 

In this project, the game at hand is Othello, a strategic board game with the goal to have the majoroty of the board covered by your colored piece by the end of the game. The project will train and test a neural network that plays against itself and determines its win percentage. Explore the code, especially the loss function in the Jupyter Notebook, and see what changes can be made to improve the win percentage.

For more about AlphaZero, please visit: https://joshvarty.github.io/AlphaZero/

# project structure

The project is made up of 6 components:

OthelloPlayers.py - Includes 3 classes, each indicating a different player type. A player can be random (one that makes a random move), greedy (one that makes the optimal move), or human (one that relies on human input to make a move). 

OthelloLogic.py - A class that sets the logic of the game. It creates everything from the board, pieces, available moves, and rules that are & are not allowed. 

OthelloGame.py - This class acts as the game itself. Once a game starts this class will know the current state of the board, the score of the game, & whether a win has been declared.

Game.py - Contains functions to be used in OthelloGame.py. The functions allow OthelloGame.py to know the state of the game as it is being played. 

Arena.py - This class initalizes and oversees the game as it is being played. It views the board at a high level, knowing whose turn it is and whether a move has won the game every step of the way.

othello_alphazero.ipynb - This notebook contains the neural network that learns how to play Othello. It uses the scripts from above, to run simulations and self learn the best possible move at a given state. Once satisified with the win percentage, the code should be transferred to a usable a python script.

# the challenge

It's encouraged for readers to clone with repo and play around with the Jupyter Notebook to improve the neural network's win percentage. At last run, the win percentage was 61%. As a starting point, check out the mean squared error loss function & see what improvements can be made. Good luck!
