# COMP-1012-Lab-8

Download Here: [COMP 1012: Lab 8](https://codingherolab.com/product/comp-1012-lab-8/)

For Custom/Original Work email codingprolab@gmail.com/whatsapp +1(541)423-7793

Question 1 (Required): Estimating the volume of a Sphere
A sphere with a radius of 1 (centered at point the point (0,0,0)) is given by the equation 1=x2+y2+z2. Click here if you want to see it visualized. This unit sphere has volume 43π units3. If you restrict this sphere to non-negative values of x,y,z, then its volume is π6 units3 which is approximately 0.524 (we got this by dividing 43π by 8). So if we were to generate a (uniformly) random point (x,y,z) in the cube [0,1)×[0,1)×[0,1), the point should have about a 52.4 % probability of landing inside the sphere because the unit cube has volume 1. This means that we can approximate π using the relative frequency of randomly generated points (x,y,z) that lie in the sphere multiplied by 6.

You are going to write a script that will estimate π by following the following steps:

Have a loop that runs TRIALS number of times, where TRIALS is the number of times we will generate points. For testing use 1,000,000 for TRIALS.
Use random.random() to generate uniformly random values from the interval [0.0,1.0). Generate one for x, one for y and one for z. This will be a give a random point (x,y,z)∈[0,1)×[0,1)×[0,1).
With your random (x,y,z) point, see if the points are within the sphere. The point (x,y,z) are in the sphere if 1>x2+y2+z2
Estimate π with π=6×# points inside sphere# of trials.
Print out your estimation of π, and the number of trials you did to get there.

Example, created with seed of 1000, your output should look like:

Estimating pi using (seed=1000)
Number of trials: 1000000, estimation of pi: 3.133602
Now increase your trials. What happens? How many trials do we need to do before we are accurate to 2 decimal places? What about 3?

Challenge (optional) – automatic precision
Write a program that will automatically increase the number of trials until you get to a specific precision. That is, ask the users how many digits of precision are required, then run trials until you reach that level of precision and report the number of trials you needed to run.

Hint: You’ll need to take the difference of the real π and the value you’re generating.

Super challenge (optional) – fixed-point arithmetic
How many digits of precision until you can’t tell the difference between what Python knows about π and the value you’re generating? Floating point numbers have limited precision on a computer. Python’s precision for integers is unlimited, and so at a certain level of precision you have to move from using floating point numbers to fixed-point arithmetic.

Convert your program to calculate π using fixed-point arithmetic.

Question 2 (Required): Rock, Paper, Scissors
Simulate a game of “Rock, Paper, Scissors”. If you are unfamiliar with the game, there is a good description on Wikipedia. In general, both players randomly choose a signal from “rock”, “paper” and “scissors”. Rock beats scissors, scissors beats paper, paper beats rock. If both players choose the same signal, it is a “push”, and neither player wins.

You can simulate a player’s choices by choosing from a list, where each element of the list is a string that is either “rock”, “paper” or “scissors”. Use random.choice to randomly choose an element from the list of signals.

Create a simulation that runs 100 rounds of “Rock, Paper, Scissors” between two players named “Right” and “Left” (think about how to represent a player abstractly – what, minimally, do you need to represent this person?). Track how many times the right wins, how many times left wins, and how many pushes there are.

Using the seed 42, your result should be:

Simulating rock, paper, scissors (seed=42)
Trials: 100, Left win %: 40.0, Right win %: 36.0, Push %: 24.0
How would the results change if left only ever uses rock?

Challenge (Optional) – No Logic
The previous problem used conditional statements extensively to determine the winner. You can write this problem in such a way that the winner is automatically determined using dictionaries and no conditional statements. Try rewriting the problem to use a dictionary of dictionaries to determine the winner of “Rock, Paper, Scissors”.

Only do this challenge if and when you have completed solving the problem with conditional statements.
