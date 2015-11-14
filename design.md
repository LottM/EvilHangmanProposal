Proposal:

HIGHSCOREVIEWCONTROLLER
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


NEWGAMEVIEWCONTROLLER
IBOutlet weak var guessedWord: UILabel

var labelGuessedWord = String()
override func viewDidLoad() {
  super.viewDidLoad()
  guessedWord = labelGuessedWord.text
}

func loadKeyboard()
func loadWordToBeGuessed()
func loadDrawingHangman()
func loadTotalAmountGuessesLeft()


CLASSES
dataHighscore = [playerName, guessedNeededToWin]
dataResumeGame = [playerName, guessedLetters, guessesLeft, displayGuessedLettersInWord, wordLength, totalAmountGuesses, evilMode]
dataNewGame = [playerName, wordLength, totalAmountGuesses, evilMode]
dataSettings = [wordLength, totalAmountGuesses, evilMode]



