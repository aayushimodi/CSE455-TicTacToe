## Webcam Based Two Player Tic Tac Toe
#### By: Aayushi Modi, Riya Baheti, Sashu Shankar

Welcome to our website for our CSE 455 Final Project: Webcam Based Two Player Tic Tac Toe!

### Introduction & Problem Set Up
Our goal was to create a program that allows you to play Tic Tac Toe by gesturing where to make your move, utilizing the webcam on your computer. Our idea was derived from Xbox Kinect and will mimic a human-camera interaction to play this two-person game. Since Xbox is not an easily mobile game and usually requires an at home setup, we wanted to build a game that can be used outside of this console set up. With our setup, one solely requires an image of an O and an X on their phone which we provide in our resources folder and can be easily downloaded onto any handheld device. This makes our Tic Tac Toe game portable and more accessible to play with friends anywhere where a laptop webcame camera is available. The game tackles interaction by using object tracking to recognize the color and shape that is held up by the player for game control.

### Process & Techniques
For this project, we used OpenCV in order to do all of our vision processing. Our code explanation explains in more detail, but OpenCV enabled us to use the webcam for our game board grid, detect contours only in a specific color range, find the enclosing circles of those contours, and pick the largest one. These steps helped us interact with the user and detect the red X or blue O that they were holding up. Beyond OpenCV, we used Python in order to run the flow of the game and keep track of the game board so we could determine who won. Lastly, we used tkinter and PIL (Python Imaging Library) in order to add start and ending screens and make our program really feel like a game in order to achieve our goal. At the bottom fo the website we have some of the resources we used for OpenCV.

### Code Explanation Video
<html>
  <video width="640" height="480" controls>
  <source src="ENTER_VIDEO_NAME_HERE" type="video/mp4">
</video>
</html>


### Demo

<html>
  <video width="640" height="480" controls>
  <source src="TicTacToeDemo.mp4" type="video/mp4">
</video>
</html>

### Gameplay Instructions
- This is a webcam based two player tic tac toe game.
- To play, click the start button to begin the game, and the tic tac toe grid will pop up.
- Make sure that one player has the red X pulled up on a handheld device, and the other player has the blue O.
- The X and O can be found in the resources folder or can be drawn as your convenience.
- The red X player starts. When it is each players' the player will hold up their device in the grid space where they would like to place their move.
- When the red X player is ready to make their move (they are holding the red X in the correct frame), they will press the r key on the keyboard to make their move.
- Similarly, when the blue X player is ready to make their move, they will press the b key on the keyboard.
- When the game is over, the winner (or a message saying that the game is a draw), will print out in the terminal.
- At this point, you can choose to play again or quit.

### Requirements to Run Code & Notes
In order to play this game, you must be using a computer with a webcam (either inbuilt or one that is plugged in should work).
In order to run the code, you may need to import some libaries (Python will error and indicate which libraries you are missing that are required for the project). Also note that for Windows users, you cannot run the program through WSL, you must run it on a Windows terminal so that the program can access the computer's webcam.

### Resources
Here are a few of the main resources we used to figure out how to do this project:
- https://docs.opencv.org/4.x/dd/d43/tutorial_py_video_display.html
- https://cvexplained.wordpress.com/2020/04/28/color-detection-hsv/#:~:text=inrange%20function%20with%20the%20range,10%20and%20160%20to%20180.
- https://docs.opencv.org/3.4/da/d97/tutorial_threshold_inRange.html
- https://docs.opencv.org/3.4/d4/d73/tutorial_py_contours_begin.html
- https://docs.python.org/3/library/tkinter.html
Beyond these we consulted other documentation for errors and smaller elements of the program that we needed to learn how to do, and lots of Stack Overflow :)
