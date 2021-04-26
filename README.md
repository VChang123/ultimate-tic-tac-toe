# CS0320 Term Project 2021

**Team Members:**  Sahil Bansal, Vanessa Chang, Samantha Hong, Emily Zhang

**Team Strengths and Weaknesses:**

Sahil Bansal:

    Strengths: Java Coding, Can work for long periods with no break, Can easily grasp concepts.
    Weaknesses: Javascript, Frontend, GUI Design, Quite Busy, Overbearing at times

Emily Zhang:

    Strengths: Frontend, GUI Design. Good logical reasoning, can go to ta hours
    Weaknesses: procrastination, overbearing at times

Samantha Hong:

    Strengths: mediocre coder, algorithms
    Weaknesses: procrastination, frontend, testing

Vanessa Chang:

    Strengths: Starts early, can write clean code. Can write good tests, can go to ta hours
    Weaknesses: Gets stressed easily, panics a lot. Not great at GUI design


**Project Idea(s):** 
### Idea 1: Ultimate TicTacToe 
https://en.wikipedia.org/wiki/Ultimate_tic-tac-toe

For students or friends who are bored and want to play a strategic game to pass the time.
Implementing 2-player Ultimate TicTacToe such that there is an option of playing against an 
intelligent player, both locally and across the web.
(If this project is not complex enough we can add more games)

Requirements:

* An easily understandable, well set up interface (with a rules page). 
Necessary for players to understand the game and have an enjoyable time playing it
    * Challenges: figuring out a way to represent different features of the game 
    (like the board, different player options, difficulty levels, etc.) in an easily understandable way.

* Predicts the next best move for the current player. An added functionality to help the players 
in the game and help the player learn different strategies. (A hint functionality)
    * Challenges: Deciding which move is the best and how to display it well in the GUI. 
      
* Use algorithms (i.e. MiniMax, alpha-beta pruning, etc.) to create the AI player (with various difficulty levels).
Necessary to implement because of the intelligent player option to allow the player to play alone when other players 
are not necessarily available.
    * Challenges: Implementing algorithms to work on a complex board and adjusting the algorithm to produce several difficulties.

* Need to create a GUI to match the players movement. Necessary for the players to interact with the game and actually use the website.
    * Challenges: Registering players movements on each respective page when players are on different devices. 
    Also setting up a clear and understandable interface

* Opponents can play on the same device or different devices. Necessary for players to have options for people to play against.
   * Challenges: Developing a connection between different devices/urls. Finding a way to host the game on a site.

**HTA Approval (dpark20):** Idea approved. Keep in mind this isn't an AI/ML class. Seems like your algorithm is not too heavily based on that though!

### Idea 2 : Manga Website
For the many people out there that enjoy reading manga and want a better platform. 
(With no advertisements and a cleaner, simpler interface)

Requirements:

* Recommender: Use an algorithm to provide recommendations based on a user's preferences. It can help the user find new things 
to read faster.
    * Challenges: Determining what to recommend (what are recommendations based on? Perhaps on genre.)

* Web Scraping: Extracts information from pre-existing websites. This is necessary in order to create the database of 
stories, as well as getting access to the information. It will be helpful to the reader because it can get the story 
that they want as long as it is out there.
    * Challenges: Creating the web scraping algorithm

* GUI to read through pages: Implement a GUI so people can actually see the book and read the information as well 
as the entire website to navigate through with its features. The user needs to be able to see the pages so this 
GUI will be helpful.
    * Challenges: Displaying each page when the user clicks the next page button or previous page button.

* Account info: necessary because there is a need to store personal information to keep people's favorite stories 
and be able to recommend new stories based on preferences. It will be much more convenient for the user to keep 
track of their current stories and updates.
    * Challenges: Finding a way to store information (must consider safety and security as well).

**HTA Approval (dpark20):** Idea approved contingent on adding more depth to your algorithmic component. How will your recommender work? The web scraper shouldn't be the main complexity of the project, so be sure to have a good algorithm for the recommender.

### Idea 3: Esoteric Language Learner
For programmers (or beginners) who want to learn the basics of a unique, niche language.
(For example, we could use Brainf*ck, Befunge, Piet)

Requirements:

* Tutorial/Lesson for different types of esoteric programming languages with interactive code snippets. 
Necessary for users to understand the basics of the language and learn in a hands-on environment.
    * Challenges: finding out what kinds of information needs to be included in a lesson. 
    Adding small code examples for users to copy and run. Another challenge is we need to learn the 
    language ourselves.
      
* Visualizer that explains what code is doing. This can be very useful for the user so they 
can see what the code is doing as in many cases esoteric languages are hard to understand and read.
    * Challenges: Hard to visualize some kinds of esoteric code: will need a different visualizer

* Parse Multiple Esoteric Languages and Executing the code. Necessary so that the user can see the 
results of the code and make changes if necessary.
    * Challenges: parsing different languages and executing them can be difficult.

* Free Space: where users can choose whichever language they want to code in and use the 
  visualizer as well. Will include a drop down menu. Necessary so users can experiment with what they learned.
    * Challenges: parsing and interpreting code that we aren’t expecting
    
* Providing simple libraries that the users can use. For example in BrainF*uck a number to 
ASCII converter. This will be more convenient for the user and give a much better coding experience
    * Challenges: Will have to code these libraries ourselves.

**HTA Approval (dpark20):** Idea NOT approved – this will either be far too difficult or far too easy (probably the former), depending on how you plan on approaching this. I think your prior ideas are better unless you narrow your scope and resubmit this proposal!

Good ideas! Looking forward to seeing what you build :)

**Mentor TA:** Katherine Sang

## Meetings
_On your first meeting with your mentor TA, you should plan dates for at least the following meetings:_

**Specs, Mockup, and Design Meeting:** COMPLETED

**4-Way Checkpoint:** COMPLETED

**Adversary Checkpoint:** COMPLETED

## How to Build and Run
* The app has been fully deployed so anyone can use the app by going to the website https://utttapp.herokuapp.com

## Design and Implementation

* **Backend**
  * Game:
  * Status:
  * IllegalMoveException:
  * Player:
  * Referee:
  * AIPlayer:
  * HumanPlayer:
  * Pair:
  * TicTacToe: 
  * RefereeTicTacToe:
  * UltimateTicTacToe:
  * RefereeUltimateTicTacToe:
  * MiniREPL:
  * UTTTGUI:
  * GameAIRoom:
  * UTTTWebsockets:
  * Main:

* **Frontend**
  * App.js: This class is the main class that creates the large scrolling page on our
    website and implements the Navbar and redirection fo the links based which
    section of the Navbar is clicked
    
  * Game.js: This class is the class that holds the main logic for playing the game. 
    It holds the logic for drawing the initial, board, converting the coordinates of the 
    pieces when a player clicks on the canvas to the corresponding place on the ultimate 
    tic-tac-toe board and switching between players.
    The more important functions are `runGame()`,  `clearGame()`, `messageHandle()`, 
    `ApplyHumanMove()`, `handleClick()`, and `AIMoveFunction()`. These functions are vital to handling
    in ensuring the correct actions are carried out depending on type of player is player
    (Human or AI) and which players turn it is. The `runGame()` function sets up the basics of the game
    when a new game is created. The `clearGame()` function resets values associated with the game and the 
    visuals whenever a new game is created so past information from older games do not interfere with newly
    created games. The `ApplyHumanMove()` and `AIMoveFunction()` functions perform the basic logic for applying
    a move to the board (like placing the move down). The `handleClick()` function is called whenever the canvas is clicked on.
    The, it determines what player the move was made by, whether the move made was valid, and whether an AI move should be 
    made in response to the human move (for Human versus AI games). The function that links everything together
    is the `messageHandle()` as it listens for the response from the backend when a message
    is sent. This function is in charge of executing its corresponding actions depending on what
    message was sent. For example, if an apply human move message was sent, the message would
    listen for a message back and see that it was an apply human move message and execute
    its corresponding actions.
    
  * Tutorial.js: This class is charge of the layout and content of the tutorial
    page on the website. It takes pictures and styles then so that they are next to a piece
    of text that explains the image or the current game scenario.
    
  * Options.js: This class handles the display and layout of all the options on the options page of the
    website. The Options class has the logic for setting the status of the players using toggles
    and whether they want to play on the same device or different device. It also 
    stores and sets the difficulty of the ai player and passes that into the Game class so that
    the Game class knows what type of game to create. 
    
  * Home.js: The class that handles the appearance and layout of the home page. The
    home page also has links to other parts of the website for quick access.
    
  * Rules.js: This class handles the content that is displayed in the Rules page of the
    website. The Rules explain how the game is played and provides basic guidence.
    
  * Referee.js: This class handles passing in the variables to both the Game and Options page.
    Both the Game and Options page are instantiated here in order to pass in variables to both
    classes because both classes need these variables. The variables set in the option class
    like what type of player player 1 is and what type of player player 2 is and if they are 
    AI players the what difficulty they are set to. These variables are used by both classes in order
    to make the correct Game so these sorts of variables are passed into both classes.
    
  * PostRequest.js: This class holds as the functions that sends the messages to the Backend websockets
    and then are exported so other classes can use them.
