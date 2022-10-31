# Homework-3
Conditional Code and Function Writing

Preface
This assignment has been structured to assess your ability to work with conditional code and write a function in R. The assignment also provides you the opportunity to translate a well-known (albeit juvenile) situation into a computer program.

Premise
As a child, you surely played a version of the game "guess the number" -- perhaps as a way of determining who gets to go first in some other game (e.g., bat first in baseball).  In this game, one person will randomly choose an integer within some bounds (say, between 1 and 20) and the other person will attempt to guess the number. You will write a function in R to mimic this game!

Directions
Write a function in R called GuessTheNumber().  This function will randomly generate an integer between a lower and upper bound (inclusive).  The user will then be prompted to enter in a guess for this number.  If their guess is too high, the function will tell the user the guess was too high and ask for another guess!  When too low, it will tell the user and ask for another guess.  The game continues until the user correctly guesses the random number. 

Specifics of the function
Your function must accept three parameters/arguments:

lower -- specifying the lower bound of the random number, defaults to 0
upper -- specifying the upper bound of the random number, defaults to 10
seed -- providing the user an opportunity to set the random number generate seed, default to NULL (thus random)
The function must do the following:

Check to make sure lower and upper are numeric values, and that lower < upper
It will stop the function and report the error in either case
Set the random number generated seed to match the user specified seed.  (use set.seed() )
The function will then perform the tasked outline above
generate a random integer
prompt the user to guess the random number, continuing until the user guesses the correct number.
The function must return a list() with the following (named) elements:

A valued called RandomNumber that reports the random number that was generated
A value called NumGuesses that reports the number of guesses the user needed
A vector called Guesses reporting the guesses the user took before (and including) the correct number

Hints and pointers

In Module 2 Part 2 we will be covering simulation and random events, but we have already covered all the code required for this assignment. Look at Day 02 - In-class - Motivating Simulation for an example that generates a random integer (effectively a die roll). Other hints:

To prompt the user for their guess, use the readline() function
An example of this function in action can be found here: readline_demo.RDownload readline_demo.R
Note: this demo is exactly that -- a demonstration!   Your function will be fairly different.
Modularize the problem!! -- Solve a simpler version of this problem first (remember, you eat an elephant one bite at a time). 
Solve the problem for a fixed "random" number (say 7) at first. 
Then get that problem working for a random number.
Then adapt that solution into a function.
Finally, work on the details needed for the function (input arguments and output list).
Use the sample() function to generate the initial random integer (see Day 02 example).
All required function & conditional code has been covered in Module 2 Part 1.
list() were covered in Module 1 Part 2.
What to submit?
You are to write your program in R but will submit the assignment through a github repository. For the canvas portion of this assignment you simply need to submit the URL for the github repository (much like we did for the Day 22 class assignment). All code for the assignment must be uploaded (or pushed) to the github repo before the end of the grace period of this assignment.

Github specifics:
Set your github repository to be private. Invite your instructor as a collaborator (tjfisher19 for Dr Fisher [section A] or MichaelHughes1963 for Mr Hughes [section B]) to this repository (otherwise it cannot be graded!!).
Your repo must include a reasonably well formatted Readme.md file that explains the purpose of the function. 
All code (.R or .Rmd) must be pushed to the repo before the end of the grace period.
Rough Rubric
Approximately 15 points will be determined by writing R code that performs the key elements of the assignment (i.e., mimicking the game). 
Generating a random number, correctly having the user guess until correct.
Approximately 10 points will be determined by following the specifications outlined in this assignment.
Writing a function with the proper arguments and output, error checking, etc...
The remaining points will be determined by following good programming practices. This includes, but is not limited to,
A properly set up Github repo (meaningful Readme.md file).
Meaningful header block in your code. 
Contextually meaningful variable names.
Scatter comments when appropriate, citations, etc...
