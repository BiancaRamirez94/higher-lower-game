# higher-lower-game

# Guess the Higher Follower Count Game
This is a simple Python program that allows you to play a game where you have to guess which of two randomly selected Instagram accounts has more followers. The game displays the names, descriptions, and countries of the two accounts, and prompts you to guess which one has more followers by typing "A" or "B".

# How to Use
Download the code to your local machine.
Run the program using a Python interpreter.
Read the descriptions of the two Instagram accounts presented to you.
Guess which account has more followers by typing "A" or "B".
If you guess correctly, the program will display your current score and generate a new set of accounts for you to compare.
If you guess incorrectly, the program will end and display your final score.

# Dependencies
This program depends on the following Python modules:

random: to randomly select Instagram accounts from a list.
art: to display ASCII art of the game's logo and comparison screen.
replit: to clear the console screen between rounds.

# Code Explanation
The game_data module contains a list of Instagram account dictionaries, each containing data about the account's name, description, country, and follower count.

The get_random_account function selects a random account dictionary from the list.

The format_data function takes an account dictionary as input and returns a string with the account's name, description, and country.

The check_answer function takes a guess ("A" or "B") and two follower counts as input, and returns True if the guess is correct (i.e. the account associated with "A" has more followers than the account associated with "B"), and False otherwise.

The game function runs the main game loop. It selects two random accounts using get_random_account, displays them to the user using format_data and ASCII art, prompts the user for a guess, checks the guess using check_answer, and updates the score accordingly. If the user guesses incorrectly, the game loop ends and the final score is displayed. To avoid repeating accounts, the function swaps the positions of the two accounts each round, as explained in the FAQ comment at the end of the code.

Finally, the program calls the game function to start the game.





