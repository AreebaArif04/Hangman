# Hangman
Overview:
Display: The Display procedure shows some introductory graphics and initializes the layout of the Hangman game, including the hangman figure and starting prompt.

Menu: The Menu procedure provides the user with four options: to play the game, view the leaderboard, read instructions, or quit the game. It prompts the user to select an option.

Game Setup: The startgame procedure randomly selects a word from predefined arrays of words (ARRAY6, ARRAY7, ARRAY8, ARRAY9) based on a generated value. This value determines which array to use. The word is stored in the wordtowork array.

Instructions: The INSTRUCTIONS procedure provides the user with details on how to play the game, such as guessing letters and the rules of the game.

Highscore Management: The CheckHighscore procedure checks whether the user has scored higher than the current highest score, adjusting it accordingly.

Graphics/Prompts: There are various sections to handle graphics or text display, including the hangman figure (Hangman array), prompts like "Press any key to continue," and displaying the current score.

Key Observations:
The game is turn-based, where the user guesses a letter and the program checks if it matches any of the letters in the word. The player can make 6 wrong guesses before the game ends.

Random Selection: The game randomly selects a word from one of four different arrays (ARRAY6 to ARRAY9), depending on the outcome of randomrange.

Menu and Options: The user can choose to play, view scores, get instructions, or quit, with corresponding logic for each option.

Next Steps or Areas to Improve:
Error Handling: It’s important to ensure that input is validated properly. For instance, if the user inputs an invalid choice, the program should prompt the user again without crashing.

Game Logic: The core logic for checking whether a letter matches the word and updating the game state (wrong guesses, word display, etc.) needs to be implemented. You will need a loop to continue asking for guesses until the player either wins or loses.

Score Calculation: Make sure the score is calculated correctly based on the number of wrong guesses and the progress in the game.

Completion of Word Selection: The word selection from the arrays (ARRAY6 to ARRAY9) is partially implemented. You will need to finish this part to ensure that words are properly selected and displayed for the player to guess.

Graphics/Output Display: The hangman graphic updates as the player makes wrong guesses. This logic should be connected with the incorrect guesses counter to display the appropriate hangman state.

Additional Recommendations:
Ensure that all strings like messages, prompts, and instructions are correctly displayed.
Consider implementing a function to handle the player's guesses and match them against the word to update the game state.
The CheckHighscore procedure can be expanded to track multiple games and persist the highest score between sessions.
