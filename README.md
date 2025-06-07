# COMPUTER-GRAPHICS-CSE423-BRACU


# Lab Assignment 1

Task 1: Drawing Pixels
You are supposed to draw 50 pixels (coordinate points). For this you need to generate
100 random values (50 x - coordinates and 50 y - coordinates). You do not need to join
any pixels for this task.

Task 2: House Building
You are to draw a House using the base primitives: points, lines, or triangles. You can
use GL_POINTS, GL_LINES or GL_TRIANGLES for designing this house. A diagram
has been provided as an example. You can modify the house design to your liking.

[![](https://i.ibb.co/wZgCMHh8/Screenshot-83.png)](https://imgbb.com/)

 Task 3: Student ID
Show your Student ID where each digit should be of different colors.


# Lab Assignment 02


🔭 Lab Assignment 2: Midpoint Line Algorithm & 8-Way Symmetry

This assignment introduces a more efficient line drawing method, the Midpoint Line Algorithm, and the concept of 8-way symmetry to handle lines of any slope.

💡 Topic Overview

The Midpoint Line Algorithm is an incremental algorithm that uses only integer arithmetic, making it significantly faster than the DDA algorithm. The core challenge is to write a single, robust function that can draw a line in any of the 8 possible zones by converting its coordinates to Zone 0, performing the calculations, and then converting them back to the original zone.

⚙️ Algorithm Details

The algorithm decides between the two possible next pixels, East (E) or North-East (NE), by checking the position of the midpoint (M) between them relative to the true line path. This avoids floating-point calculations and relies on a simple decision parameter.

📝 Activity Task

Objective: Draw the last two digits of your student ID.

Implementation: You must implement the Midpoint Line Algorithm with 8-way symmetry to handle all the lines required to draw the two digits.

Example Output:

For a student ID ending in 06, the output should look like this:




# Lab Assignment 03


🎨 Lab Assignment 3: Midpoint Circle Algorithm
This lab builds upon the concepts of the Midpoint Algorithm and 8-way symmetry, applying them to efficiently draw circles.

💡 Topic Overview
Similar to the line algorithm, the Midpoint Circle Algorithm uses a decision parameter and integer arithmetic to determine the closest pixel to the true circle path at each step. By calculating the pixels for just one octant (1/8th of the circle), we can use the 8-way symmetry of a circle to plot the points for the other seven octants without re-calculation, making the process highly efficient.

📝 Activity Task
Objective: Draw a flower-like pattern using multiple intersecting circles.

Implementation: Implement the Midpoint Circle Drawing algorithm. The final output should replicate the provided image, which consists of one large circle and eight smaller circles forming a rosette pattern.

Example Output:




# PROJECT


# Facial Expression Simulator

An interactive OpenGL program that displays various facial expressions with animation capabilities.



## Features

- Displays 6 different facial expressions:
  - Happy 😊
  - Sad 😢
  - Crying 😭
  - Neutral 😐
  - Laughing 😂
  - Smirk 😏
- Includes an animated rotating "Joker Face" (option 7)
- Uses midpoint algorithms for drawing lines and circles
- Interactive menu system

## Requirements

- Python 3.x
- PyOpenGL
- NumPy
- FreeGLUT (for Linux/Mac) or equivalent OpenGL utilities

When prompted, enter a number (1-7) corresponding to the emotion you want to display:

################
Facial expression based on current emotion: 
1) Happy 
2) Sad 
3) Crying 
4) Neutral 
5) Laughing 
6) Smirk 
7) Rotating Joker Face trying to more laugh (Animated)
What's your emotion right now? Enter:


## Technical Details:

Uses midpoint line and circle drawing algorithms

Implements zone conversion for line drawing in all octants

Includes matrix transformations for rotation animation

Built with:

OpenGL for rendering

GLUT for window management

NumPy for matrix operations

