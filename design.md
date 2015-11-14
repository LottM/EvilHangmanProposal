#Proposal:

###HighscoreViewController
    class highscore {
      var playerName: String?
      var guessesNeededToWin: Integer?
  
      func highscoreData() {
        var dataHighscore = []
        if let playerName = self.playerName {
          dataHighscore += [playerName]
        }
        if let guessesNeededToWin = self.guessesNeededToWin {
          dataHighscore += [guessesNeededToWin]
        }
        return " ".join(dataHighscore)
      }
    }


###NewGameViewController
    @IBOutlet weak var guessedWord: UILabel

    var labelGuessedWord = String()
    override func viewDidLoad() {
      super.viewDidLoad()
      guessedWord = labelGuessedWord.text
    }

    func loadKeyboard()
    func loadWordToBeGuessed()
    func loadDrawingHangman()
    func loadTotalAmountGuessesLeft()

    if evilMode(sender:UISwitch) = on {
      funcDictionaryEvilMode()
    }
    else {
      funcDictionaryNonEvilMode()
    }

    if letterIsGuessedRight() == True {
      func colorLetterGreen()
    }
    else {
      func colorLetterRed()
    }

###SettingsViewController
    @UITextfield: wordLength (integer?)
    @UITextfield: totalAmountGuesses (integer?)
    @UISwitch: evilMode

###Classes
    dataHighscore = [playerName, guessedNeededToWin]
    dataResumeGame = [playerName, guessedLetters, guessesLeft, displayGuessedLettersInWord, wordLength, totalAmountGuesses, evilMode]
    dataNewGame = [playerName, wordLength, totalAmountGuesses, evilMode]
    dataSettings = [wordLength, totalAmountGuesses, evilMode]

#####Model classes
![GitHub Logo] (http://s19.postimg.org/5nvfsstcj/Model_View_Controller.png)

#####MenuViewController
![GitHub Logo] (http://s19.postimg.org/cl3utxaqb/Menu_View_Controller.jpg)

#####HighscoreViewController
![GitHub Logo] (http://s19.postimg.org/ldkthlvv7/Highscore_View_Controller.jpg)

#####SettingsViewController
![GitHubLogo] (http://s19.postimg.org/acpocl3mb/Settings_View_Controller.jpg)

#####NewGameViewController
![GitHub Logo] (http://s19.postimg.org/lnsc0yahf/New_Game_View_Controller.jpg)

#####ResumeGameViewController
![GitHub Logo] (http://s19.postimg.org/8ap6yc5n7/Resume_Game_Viw_Controller.jpg)




