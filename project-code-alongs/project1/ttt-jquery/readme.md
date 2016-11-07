# Project 1 Code Along

## index.html

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Tic Tac Toe</title>
  <link rel="stylesheet" href="app.css" media="screen">
</head>
<body>
  <section>
    <h1>Tic Tac Toe!</h1>
    <div id="board" class="container well"></div>
    <p id="statusMessage"></p>
    <button class="btn btn-primary btn-large" onclick="game.reset()">New Game</button>
  </section>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js" charset="utf-8"></script>
  <script src="app.js" charset="utf-8"></script>
</body>
</html>
```

## app.css

```css
* {
  text-align: center;
  font-family: "Courier"
}
button {
  background-color: white;
}
.X {
  color: green;
}
.O {
  color: red;
}
```

## app.js

```javascript
var game = {
  board: null,
  $board: null,
  $statusMessage: null,
  currentPlayer: 'X',

  togglePlayer: function() {
    this.currentPlayer = (this.currentPlayer === 'X' ? 'O' : 'X');
  },

  showCurrentPlayer: function() {
    this.$statusMessage.text('Current Player: ' + this.currentPlayer);
  },

  showWinner: function() {
    this.$statusMessage.text('Player ' + this.currentPlayer + ' has won!');
  },

  showCat: function() {
    this.$statusMessage.text('CAT!!!');
  },

  checkForMatch: function($cell1, $cell2, $cell3) {
    return $cell1.text() === $cell2.text() &&
           $cell1.text() === $cell3.text() &&
           $cell1.text() !== '?';
  },

  move: function(r, c) {
    // alert('you move me: ' + r + ',' + c);
    this.board[r][c].text(this.currentPlayer).addClass(this.currentPlayer).prop("disabled", true);
    if (this.checkForEndOfGame() === false) {
      this.togglePlayer();
      this.showCurrentPlayer();
    }
    else if (this.winner) {
      this.showWinner();
      $('.cell').prop("disabled", true);
    }
    else {
      this.showCat();
      $('.cell').prop("disabled", true);
    }
  },

  isBoardFull: function() {
    for (var r=0; r<3; r++) {
      for (var c=0; c<3; c++) {
        if (this.board[r][c].text() === '?') {
          return false;
        }
      }
    }
    return true;
  },

  checkForEndOfGame: function() {
    var rowMatch  = this.checkForMatch(this.board[0][0], this.board[0][1], this.board[0][2]) ||
                    this.checkForMatch(this.board[1][0], this.board[1][1], this.board[1][2]) ||
                    this.checkForMatch(this.board[2][0], this.board[2][1], this.board[2][2]);
    var colMatch  = this.checkForMatch(this.board[0][0], this.board[1][0], this.board[2][0]) ||
                    this.checkForMatch(this.board[0][1], this.board[1][1], this.board[2][1]) ||
                    this.checkForMatch(this.board[0][2], this.board[1][2], this.board[2][2]);
    var diagMatch = this.checkForMatch(this.board[0][0], this.board[1][1], this.board[2][2]) ||
                    this.checkForMatch(this.board[0][2], this.board[1][1], this.board[2][0]);
    this.winner = rowMatch || colMatch || diagMatch;
    this.cat = !this.winner && this.isBoardFull();
    return this.winner || this.cat;
  },

  buildGameBoard: function() {
    this.board = [];
    for (var r = 0; r < 3; r++) {
      var $row = $("<div></div>");
      var row = [];
      for (var c = 0; c < 3; c++) {
        var $button = $('<button class="btn-lg cell" onclick=game.move(' +
            r + ',' + c + ')></button>');
        row.push($button);
        $row.append($button);
      }
      this.$board.append($row);
      this.board.push(row);
    }
  },

  reset: function() {
    $('.cell').text('?').removeClass('X O').prop("disabled", false);
    this.currentPlayer = 'X';
    this.winner = false;
    this.cat = false;
    this.showCurrentPlayer();
  }
}

$(function() {
  game.$board = $("#board");
  game.$statusMessage = $("#statusMessage");
  game.buildGameBoard();
  game.reset();
});
```
