In order to run this application, download the entire folder "CellaAnt12" and open the CellaAnt12.html file located in the folder in any web browser. 

Cella Ant 12 
William Timani

Intro:
This is a javascript program, with html incorporation for display, that visualizes Langton's Ant. In this case it is Turk & Propp's Ant #12. This ant moves based on the color of the square under it. If the color is black or red, it turns right. If the color is yellow or blue, it turns left. Each time it moves it changes the color of the square under it to the next color in the sequence. The sequence of colors is black, red, yellow and blue. After blue, the cycle repeats. The ant runs for a set amount of moves and each move is shown on a grid. 

The algorithm consists of a loop that runs through each move of the ant. By default it loops 10000 times. In the loop, the algorithm first checks for the color of the 10x10 square under the ant using the image data of the ant's current x and y position. It runs through a series of if statements checking if the image data is one of the colors in the cycle(black,red,yellow,blue) using the color codes of the image. Once it has found the color of the square is changes the color of it to the next color in the sequence. Next, the ant turns right(if black or red) or left(if yellow or blue) using a turn() function. The turn function takes in the direction to turn(0 is right, 1 is left), current heading of the ant(n,s,e,w) and the context variable of the canvas. Inside the turn function, the direction that the ant is turning is first checked. Based on if it is turning left or right and taking in to account the current heading of the ant, it will translate in the proper x or y direction 10 units. A new heading is returned to the caller based on the turn and that heading is stored as the new current heading. The last action performed in the loop is the adjust the ant's current x and y position based on the new heading. 

Contents:
CellaAnt12.html
draw-stuff.js
styles.css
README.txt
ComplexityTimeReport.pdf

External Requirements:
Google Chrome was used to test this program, however it should work in most modern web browsers.

Setup and Installation:
No installation required (unless you do not have a modern web browser). Simply open the CellaAnt12.html file or drag it onto the web browser of choice.

Sample Invocation:
The program is started and the ant begins moving. It will continue to move for 10000 moves and the speed can be changed dynamically during the program. 

Features:
- "Ant" in the form of a colored 10x10 square moving across a 410x410 grid

- Ant changes color of the square under it as it moves based on a sequence: black,red,yellow,blue

- Ant turns right on red and black squares and left on blue and yellow squares

- Change the speed of the ant dynamically 

Bugs:
- No known bugs

Third Party Material:
draw-stuff.js, styles.css and small parts of CellaAnt12.html were provided by Charles Siska

![CellaAntPic](Images/CellaAntPic1.png)
