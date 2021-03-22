### @explicitHints true

# Turtle Logo - Lesson #7

## Turtle Logo - Lesson #7 @unplugged
**Making the Turtle do Spirograph.**

In this lesson you will use loops, to make Spirograph images.
![loop](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson7/raw/main/assets/spirograph_screenshot.png)

## Step 1
** Follow Along**

Once again, all our programs begin with an ⇢``on start``⇠ block. Then you need to add the **Turtle** using the ⇢``show turtle``⇠ block.
```blocks
turtle.showTurtle()
```

## Step 2
** Follow Along**

You know from previous lessons how to move forwards and backwards. But you can also just move the **Turtle** directly to a specific location. To do this we use the ⇢``set turtle's position (x 0, y 0)``⇠ block. (0,0) is the center of the screen.
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(0, 0)
```

## Step 3
**Try it out**

Try moving the **Turtle** around the screen. Use positive and negative numbers.
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-43, -13)
```

## Step 4
** Follow Along**

You also know how to turn the **Turtle**. You know if you turn the **Turtle** 90° 4 times you get a square. (Remember, loops are your friend!)
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-25, 20)
for (let index = 0; index < 4; index++) {
    turtle.moveTurtleDirection(TurtleDirection.Forward, 50)
    turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
}
```

## Step 5
** Try it out**

But what would happen if you turn the **Turtle** more than 90°? Give it a try and see what happens. (Pick an angle larger than 90° but less than 360°.)
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-25, 20)
for (let index = 0; index < 4; index++) {
    turtle.moveTurtleDirection(TurtleDirection.Forward, 50)
    turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 280)
}
```

## Step 6
** Follow Along**

It might not look exactly like you want. You might have to change the starting location of the **Turtle**, so it does not go off the screen. You might have to increase the number of times it does the loop. You might want to increase the size of steps it takes. You might need to change the turning angle to adjust things. All of this is OK. 
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-35, -40)
for (let index = 0; index < 9; index++) {
    turtle.moveTurtleDirection(TurtleDirection.Forward, 70)
    turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 280)
}
```

## Step 7
** Follow Along**

You can even move the **Turtle** back to the center when it is done, with the ⇢``move turtle home``⇠ block. 
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-35, -40)
for (let index = 0; index < 9; index++) {
    turtle.moveTurtleDirection(TurtleDirection.Forward, 70)
    turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 280)
}
turtle.home()
```

## Step 8
**Success!**

You can now use loops, to make your own Spirographs.

## Step 10
**Your Turn**

Get your **Turtle** to draw a your own Spirograph. Ensure it:
- is not using 280° but is larger than 90° (turns out even numbers are better!)
- change the color of the pen
- fill your screen as much as possible
- center your Spirograph as much as possible
- return the **Turtle** to the center when done
- loop enough times that you end up back where you started
- say, "Spirograph" at the end

## Step 11
**Done**

You have successfully completed your six lesson in Turtle Logo.

```ghost
turtle.say("Hello, World!")
turtle.showTurtle()
turtle.setPositionCartesian(0, 0)
for (let index = 0; index < 4; index++) {
}
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.home()
```
