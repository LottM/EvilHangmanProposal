# EvilHangmanProposal
This is a proposal for the second assignment: Evil Hangman, in which the computer changes the word to be guessed when possible.

### Bulleted list of features
* dictionary for words.plist
* UILabels displaying amount of guesses, guessed letters and open letter positions
* UITextField for prompting the user for input, thereby only accepting alphabetical characters
* for loop iterating over values in dictionary comparing them to users input
* UITabBarController for tabs below (settings, new game)
* UIImage for logo
* UISlider for length of words, maximum number of guesses 
* UISwitch for evilness
* UITabBarController for highscores

### Short pseudocode thoughts
Include words.plist

Display guesses, guessed letters and open letters
Get input user via UITextField
if !isalpha(input):
  print: Try again! That wasn't an alphabetical letter.

do: 
  if (wordsWithLetter > wordsWithoutLetter):
    newList = wordsWithLetter
  else:
    print: Too bad! Guess again.
while (guessed != true)

if (guessed == true):
  print: Unbelievable! You won! Congratulations!
  return 0
else:
  print: Too bad, you've lost!
  return 0
