Proposal:

HIGHSCOREVIEWCONTROLLER
class highscore {
  var playerName: String?
  var guessesNeededToWin: Integer?
  
  func highscoreData() {
    var data = []
    if let playerName = self.playerName {
      data += [playerName]
    }
    if let guessesNeededToWin = self.guessesNeededToWin {
      data += [guessesNeededToWin]
    }
    return " ".join(data)
  }
}
