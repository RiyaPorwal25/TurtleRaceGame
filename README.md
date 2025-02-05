# TurtleRaceGame
It is an game of turtles race ,where you choose how many number of player(turtle) will be racing.  Then the game begins ,in end the winner's name will be dispalyed

The description of program is-
1. Constants and Setup:
WIDTH and HEIGHT: Define the size of the race area (500x500 pixels).
COLORS: A list of possible colors for the turtles (red, yellow, green, etc.).
2. get_number_of_racers():
This function asks the user to input the number of turtles they want in the race (between 2 and 10).
It checks if the input is valid (numeric and within the range). If not, it keeps asking until valid input is given.
3. race(colors):
This function simulates the race.
It calls create_turtles(colors) to generate turtles.
Inside a loop, each turtle moves forward by a random distance (between 1 and 20 pixels).
The race continues until one of the turtles crosses the finish line (approaching the top of the screen), which is set to y >= HEIGHT//2 - 10.
When a turtle reaches the finish line, the function returns the color of the winning turtle.
4. create_turtles(colors):
This function creates and sets up each turtle.
It positions each turtle at the bottom of the screen in evenly spaced positions.
Turtles are given their respective colors, shapes, and initial positions.
5. in_turtle():
This function sets up the turtle graphics screen.
It defines the window size (WIDTH, HEIGHT), the window title, and prepares the screen for the race.
6. Main Code Flow:
First, the number of racers is determined by calling get_number_of_racers().
Then, in_turtle() initializes the turtle graphics window.
The colors list is shuffled, and the appropriate number of turtles are chosen.
The race() function is called to run the race, and the winner is printed at the end.
Example Execution:
The program asks for the number of turtles.
It then initializes a graphical window and starts the race.
Each turtle moves randomly, and the first one to reach the finish line is declared the winner.
This code effectively simulates a simple turtle race using random movement and displays the winner's color in the console.
