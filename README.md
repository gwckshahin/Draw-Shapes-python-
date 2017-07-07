# Shapes
Here is the code for python:

from turtle import *
import math

# Name your Turtle.
timmy = Turtle()

# Set Up your screen and starting position.
timmy.penup()
setup(500,300)
x_pos = -150
y_pos = -150
timmy.setposition(x_pos, y_pos)
timmy.speed(10)

### Write your code below:
sides=int(input("Insert the amount of sides you want your polygon to have"))
answer=input("What color do you want your shape to be?")
fillcolor(answer)
def polygon(sides, length):
    for x in range(sides):
        pencolor(answer)
        forward(length)
        right(360/sides)

timmy=True
while timmy==True:
    if sides == 0:
        timmy= False
    else:
        clear()
        begin_fill()
        polygon(sides,100)
        end_fill()
        timmy=False


done()

# Close window on click.
exitonclick()