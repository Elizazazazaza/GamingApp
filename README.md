**CSC207 Phase 2 README.md**

Welcome to our Phase 2 Project. In this project, we implemented an app that contains three games: a turn-based RPG named Ghost Hunt, a puzzle-solving game called Sliding Tiles, and a mathematical logic challenge - Sudoku. We hope that you have fun playing them. We implemented these games using a Model-View-Controller design while closely following the guidelines of SOLID principles. These three games are packaged into a &quot;Game Center&quot; where they can be accessed. Each registered user of the app will also have access to their personal profile - an interface that displays the user&#39;s highest scores and allows them to edit information such as the profile image and password.

**Source:** https://markus.teach.cs.toronto.edu/git/csc207-2018-09-reg/group\_0640

**Prerequisites:**

To run the app, you will need to install Android Studio on you machine.  Also, you will need to download Virtual Device Pixel 2 API 27 in Android Studio. To ensure a smooth app experience on your Windows platform,  Intel® Core™ i9 7980XE and NIVIDIA 2080RTX are recommended, but you can probably make do without them.

**Playing the Games:**

When the app is ran with emulator, you will then be taken to an interface where a login prompt is displayed. If you are opening this project for the very first time, you will not be able to login since you do not have a signed-up account. To obtain an account, kindly click on &quot;Sign up here&quot; icon which will send you to the sign-up page.

You will need a username and a password. Please use a permutation of uppercase letters, lowercase letters and underscores for your username. Although we are not too concerned with user privacy and security, we still recommend that your password consists of an eight-digit alphanumeric permutation so that your beloved gameplay information does not fall into the wrong hands.

Then, simply login and you will be taken to the &quot;Game Center&quot; page. Here you will have access to our games and your profile. By clicking on &quot;User Center&quot;, you will be taken to your personal profile page. Here you can view your highest scores for each of the games. You can also change your password here. Finally, if you, for some unimaginable reason, happen to dislike the default profile picture, you can also change it here.

Returning to the &quot;Game Center&quot; page, if you choose to click on any of &quot;Ghost Hunt&quot;, &quot;Sudoku&quot;, or &quot;Sliding Tiles&quot; button, you will be taken to that game&#39;s starting page.

In your first run through the program, there will not be any loaded games. However, you will have the option to save an unfinished game and load it from this page later.

A scoreboard can also be accessed from the Game Center via button click. On it, the current player&#39;s ranking and score will be displayed along with the top 5 tryhards. If the app is opened for the first time, there will be no data recorded.

When you start a new game, a new page will appear. We believe that the games are straight forward enough that they do not require lengthy descriptions. Try clicking around, magical things will happen.

Note: turn emulator to landscape, lay on your side, or turn you machine sideways while playing Ghost Hunt.

After a game is finished, a scoreboard will be displayed, and hopefully you have moved up the ranks.

**All Implemented Functionalities (explicitly required):**

- Code coverage where applicable (unit test)
- Always generate a solvable SlidingTiles game board (SolvableGenerator.java class in slidingtiles folder)
- Added two games and accommodating scoreboards
- Per-user scoreboard
- Undo feature for at least one of the new games (Ghost Hunt undo five moves)
- Autosave for at least one of the new games (Sudoku and Ghost Hunt)
- Design Pattern implementations (see Design Pattern Usage section)
- Updated test cases along with refactoring

**All Other Functionalities (Features):**

- Signup page
  - Used regular expression to restrain username to a permutation of uppercase letters, lowercase letters, and underscores. This ensures that usernames can be written into  valid file names.
- Login page
- Game Center page
- User Center
  - Change Profile Picture
    - Default picture as our beloved Professor Danny Heap
  - Change Password
  - ListView format of per-user scoreboard can be scrolled down
- Sliding Tile Game
  - Displays current play name
  - Displays number of moves
  - Change Background
- Sudoku
  - Autosave on every move
  - Three levels of difficulty
  - Displays current play name
  - When a visible cell is selected, all other cells with the same value becomes highlighted.
  - Maximum three hints provided
  - Incorrect placement of numbers are displayed and taken into account in score calculation
  - Toast &quot;Wrong Answer&quot; becomes a more severe warning after four wrong answers
- Ghost Hunt
  - Autosave on the start of every level
  - Manual save game function
  - Restart level (player receives fresh undos but the number of moves does not reset)
  - Ghost AI that follows the player along a trajectory that is closest to a straight line
  - Ghost cannot catch player at the exit
  - Beating the levels and failing levels produces different end-game Toasts
- Overall visual upgrade

**Running the Tests:**

We have written unit tests for all Controller in our Model-View-Controller design. They can be found under the folder fall2018.csc2017.game\_centre(test).

These tests are written to ensure that our algorithms produce the desired results.

**Built With:**

- Android Studio
- Git
- Github and StackOverflow (all external sources are cited)

**Authors:**

Please read TEAM.md for more information

**Acknowledgements:**

- To my awesome teammates, for making this possible
- To Ma Youxuan&#39;s childhood, for coming up with the idea of Ghost Hunt
- To Billie Thompson at PurpleBooth, for this template
- To our beloved Professor Danny Heap, for being the default profile photo
- To you, for reading, marking (and possibly smiling at) this.

**Support:**

Contact our support team at [tempsucker@gmail.com](mailto:tempsucker@gmail.com) (usually reply sooner than remark requests).

**Things to note:**

- If you accidentally venture into an undesirable page, simply click on the &quot;Back&quot; button to get out of there. In the event where no &quot;Back&quot; button is found, click on the back key on the emulator.
- When starting a new game of Sliding Tiles, you will be prompted to choose the size of the board (integer between 3-5) as well as the maximum number of undos. Please understand that the larger your board, the game will likely be more difficult, and your score will be adjusted accordingly so that, when compared to the scores from a less difficult run of the game, you are not at a disadvantage. The same goes for your score between a difficult and easy game of Sudoku.
- There are no bugs, only features. Some will, perhaps, seem counterintuitive. However, no matter how much they seem like bugs, they are, in fact, features.
