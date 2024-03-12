# Fruity Pairs Fiesta
startup application for CS 260
## Specification Deliverable
### Elevator Pitch
These days, it seems that kids' attention span is getting worse and worse with TV shows and games that provide constant stimulation. Fruity Pairs Fiesta is a memory exercise for kids that will strengthen their minds and sharpen their focus overall.
### Design
![Mock](FruityPairsHome.png)
![Mock](FruityPairsGame.png)
![Mock](FruityPairsLeaderboard.png)
### Key Features
- Secure login over HTTPS
- Displays Leaderboard with live updates
- Stores individual best scores (lowest time)
### Technologies
I will use the following technologies in the following way:
- HTML - Used to create the game board and score display.
- CSS - Used to create the visuals so it is more visually appealing.
- Javascript - Provides login, handles interaction on the page, and game logic/processes such as timers.
- HTTPS - Enables secure login.
- DB - Stores login information and best scores.
- WebSocket Data - As users get better scores, the highest scores are. broadcasted on the leaderboards page live.

## HTML deliverable
For this deliverable I built out the structure of my application using HTML.

HTML pages - Three HTML page that represent the ability to login, play the game, and view a leaderboard of scores.
Links - The login page automatically links to the play page and the scorebaord page. The scoreboard and play pages also have links to one another.
Text - There is textual data in the title and in the leaderboards.
Images - I imported several pictures of fruit to go along with the theme of Fruity Pairs Fiesta! I included them both in the play page and on the home page.
DB/Login - Input box and submit button for login. The login information will pull from a database of the users.
WebSocket - The leaderboard will provide live updates with WebSocket data.

## CSS deliverable
For this deliverable I properly styled the application into its final appearance.

Header, footer, and main content body
Navigation elements - I dropped the underlines and put them at convenient locations and changed the hover color
Responsive to window resizing - My app looks great on all window sizes and devices, the images disappear if the window is too small, and the buttons go into different sizes of rows/columns so it will fit the screen
Application elements - Used good contrast and whitespace
Application text content - Consistent fonts
Application images - They size and are removed if the window is too small. Good icons