# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project #1: Let the Games Begin

## PROJECT Requirements

For your first project you will build a simple game as a Web Application. You may choose from one of the ideas listed below or you may choose another game __with approval from one of the WDI instructors__.

### Project Objectives

The objectives of this project are to:

* Demonstrate your ability to use `HTML` and `CSS` to build and style an intuitive web application
* Demonstrate your competancy in _DOM manipulation_ using JavaScript
* Publish your source code to _GitHub_ with a solid `README.md` describing the project
* Deploy your application to a production environment such as [GitHub Pages](https://pages.github.com/) or [BitBalloon](https://www.bitballoon.com/)
* Present your project in an _science fair_ / _meet-and-greet_ style format

## Project Ideas

### Connect 4

![Connect 4](images/connect-4-game.jpg)

Write a _Connect 4_ game that allows two players to compete. The players are sharing the same computer but the game detects when a player has won the game. A scoreboard keeps track of how many times Player 1 has won and how many times Player 2 has won.

#### Bonuses:

* Alternate the first player to move: Player 1 moves first in game 1, Player 2 moves first in game 2, etc.
* Allow players to enter their name and display their name instead of "Player 1" and "Player 2".
* Provide a way to play against the computer (using a simple A.I. algorithm)

---

### Simon

![Simon Game](images/simon-game.jpg)

Write a _Simon_ game that displays 4 colored buttons (or clickable areas) that light up and play a sound. Have the computer play a random sequence, starting with a length of 1 and growing with each round. If the user can replay the sequence by clicking on the colored buttons in the correct order, then the computer goes to the next round and the sequence gets longer (same sequence but with one new randomly generated selection added to the end). If the user is unable to replay the sequence, then their score is the length of the sequence they successfully replayed.

Have a unique sound for each colored button and play the sound both when the computer plays the sequence and when the user clicks on the buttons to replay the sequence. Have a special sound for when the user makes a mistake.

#### Bonuses:

* Display a scoreboard of the longest sequence successfully played to date.
* Have a way for the user to choose the difficulty (`easy`, `medium`, or `hard`) where the `easy` mode plays the sequence slowly (one second per highlighted button) and the `hard` mode plays the sequence more quickly (1/4 second per highlight).

---

### Hangman

![Hangman Game](images/hangman-game.gif)

Write a _Hangman_ game that displays a secret word as a list of hidden letters. Also display an alphabet of letters that the user can guess while trying to guess the word. After a letter is used, disable that letter from the alphabet so the user will not try to guess the same letter twice. When a guess matches one or more letters in the secret word, reveal those letters to the user. Keep track of the number of incorrect guesses and end the game if the number of incorrect guesses reaches 6. If the user reveals all of the hidden letters before reaching 6 incorrect guesses, then the user wins.

#### Bonuses:

* Display a _hangman_ as either ASCII art or images that represent the various stages of the _hangman_.
* Display a scoreboard of how games won and lost.
* Choose a theme for the game, such as "Famous Movies" or "Web Development Terms"

---

### Jeopardy

![Jeopardy Game](images/jeopardy-game.jpg)

Write a _Jepardy_ game that allows the user to play the game of _Jeopardy_. This is basically a quiz where the user gets to choose the next question by choosing from a category and then choosing a point amount (100 to 500). The questions are phrased as answers and the user chooses from a list of 4 questions that match the answer. For instance:

The User sees this: `A programming construct for easily looping through the elements in an array`
The User chooses this: `What is a for loop`

#### Bonuses:
* Have a "Round 1" and a "Round 2" where the questions in Round 2 are more difficult but also score higher points.
* Have different themes for the questions, such as:
  - Web Development Topics
  - Arts and Entertainment
  - Science and Science Fiction

---

### BlackJack

![BlackJack Game](images/blackjack-game.png)

Write a _BlackJack_ game to try to beat the dealer. Allow the user to place a bet (using chips, points, or dollars). Allocate a starting amount of chips and keep track of the user's chip count. If the user beats the dealer without busting, the user doubles their bet in chips. Otherwise the user loses their bet. Follow the common rules for _BlackJack_.


## Bonuses for Any Game

* Keep score
* Make it responsive
* Add A.I. (player vs. computer)
* Add a timer
* Add music while a player makes a choice
* Create a theme via background images, sounds, music, avatars, etc.
  - Star Wars
  - Favorite Sports Team or Rivalry
  - Comic Book Characters
* Add avatar choices for the player
* Implement multiple games on your site


## Planning and Deliverables

### Project Plan Deliverables (Due at time of Presentation):

* All source code is checked into GitHub
  - create a repo for your app and show that you've been commiting early and often while utilizing clear commit messages.
* A `README.md` file containing:
  - A Project description
  - A Link to the Deployed App
  - A Link to the Trello Board
  - A Link to any Wirefames or Mockups (or inline photos / screenshots will work too!)
  - A list of technologies, libraries, and/or frameworks used in the project, such as `Twitter Bootstrap`, `jQuery`, or `Animate.css`
* Wireframes or Mockups -- what does the app look like?
  - Simple: take a picture of a whiteboard drawing
  - Advanced: use a tool such as [Balsamiq](https://balsamiq.com/) or [Mockingbird](https://gomockingbird.com/home)
* User Stories in [Trello](https://trello.com/)
  - You should have a Trello board tracking your User Stories
  - Board lists should include:
    * Backlog
    * Todo
    * In Progress
    * Under Review
    * Done

### Sample Project `README.md` files:

* [Tic-Tac-Toe](https://github.com/iamsydsmith/tic-tac-toe)
* [FootUp](https://github.com/wschaeferiii/footup)

## Technical Requirements

Your app must:

* Render a game in the browser
* Use Javascript or jQuery for DOM manipulation
* Switch turns between two players and/or use some A.I. to control the game.
* Design logic for winning & visually display which player won
* Include separate HTML / CSS / JavaScript files
* Write high quality code:
  - Follow accepted naming conventions
  - Consistent indentation
  - Well-structured and readable code
  - Semantic naming of variables, functions, CSS classes, etc.
  - Short and clear functions that _do one thing_
  - Efficient code (cache references to DOM nodes, etc.)
  - DRY (Don't Repeat Yourself) code
* Deploy your game online, where the rest of the world can access it
* Use semantic markup for HTML and CSS (adhere to best practices)

## Suggested Ways to Get Started

* First design your _MVP_ (Minimum Viable Product). Have a plan for completing an MVP before getting too involved with _advanced_ features.
* Use _Trello_ to prioritize your User Stories / features. Focus on what is most important / critical to success.
* _Timebox_ any experimental or optional ideas, features, or technologies. Remember that good _time management_ is key!
* Commit your code early and often with good commit messages.
* Use Git Branching for experimenting with different ideas and technologies.

## Project Feedback + Evaluation

Your project will be evaluated by your instructional team in order to provide you with useful feedback. The following criteria will be used for the evaluation:

* __Project Workflow__: Did you complete the user stories, wireframes, task tracking, and/or ERDs, as specified above? Did you use source control as expected for the phase of the program you’re in (detailed above)?

* __Technical Requirements__: Did you deliver a project that met all the technical requirements? Given what the class has covered so far, did you build something that was reasonably complex?

* __Creativity__: Did you add a personal spin or creative element into your project submission? Did you deliver something of value to the end user?

* __Code Quality__: Did you follow code style guidance and best practices covered in class, such as spacing, modularity, and semantic naming? Did you comment your code as your instructors have in class?

* __Deployment__: Did you deploy your application to a public url using GitHub Pages or something equivalent?

* __Total__: Your instructors will give you a total score on your project between:

    Score | Expectations
    ----- | ------------
    **0** | _Incomplete._
    **1** | _Does not meet expectations._
    **2** | _Meets expectations, good job!_
    **3** | _Exceeds expectations, you wonderful creature, you!_

 This will serve as a helpful overall gauge of whether you met the project goals, but __the more important scores are the individual ones__ above, which can help you identify where to focus your efforts for the next project!
