# hangman

## Description
This is a README.md file for my Hangman project. It was done on Visual Studio Code through the
GitHub repository. On Visual, the program can be run with the following command:

`node .`

Once the enter key has been pressed, the game starts, and the program will pick a random word
from a word bank of many different words in the word-bank.json file. The user will be provided a number of
underscore characters for each letter in the chosen word, with whitespaces between underscores.
They will also be provided with the number of tries they have remaining. The user starts off with 6 tries.

The code puts the word in two different formats, an array format and a string format. The string format is used
when checking the user input.

Whenever the user guesses a letter, that letter will be stored into an array called alreadyguessed
that stores all of the letters the user has guessed so far. If the letter is in the puzzle, the letters will be
filled in the correct places. If the user guesses a letter that they have already guessed, the program will tell
them that they have already guessed that letter (this would not count against the user).
If the letter isn't in the puzzle, the program will tell the user that there is no instance of that letter,
and the player will lose 1 of their tries. Also, if the user types in more than
one letter and presses enter, the program will only use the first letter in the input and ignore the rest.

If the user manages to fully guess the word, the program will congratulate the player, give them a win, and start a new round.
However, if the user has no more tries, the round ends, the word is revealed, and a new round starts. In both cases, the program
will keep track of how many games they have played so far.

In order for the user to exit the program, they have to input this command:

`^C`

Here are some more things to learn about this program:
* If the user inputs an uppercase letter, that letter will automatically be converted to lowercase.
* If the user inputs a non-alphabetic character (like a number), that character will be ignored by the program.
* The array that stores all of the letters that the user guesses in each round, alreadyguessed, will be emptied out before a new round starts. This also applies to the chosen word in both array and string formats. In addition, the number of tries gets reset to 6.
* Three arrow functions have been used throughout the javascript file, index.js.
* The higher-order function, `forEach`, has been used three times throughout the index.js file.
* Comments have been provided throughout the code for simplification purposes.
