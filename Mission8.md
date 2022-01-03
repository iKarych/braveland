# Mission 8
```package
maqueen=github:dfrobot/pxt-maqueen
```

## Introduction @unplugged

In this mission, you will learn how can you make functions to make your life easier when programming!

## Step 1

First, solve the maze and code the solution as you would normally do:

- go straight
```blocks
maqueen.motorRun(maqueen.Motors.All, maqueen.Dir.CW, 100)
basic.pause(400)
maqueen.motorStop(maqueen.Motors.All)
basic.pause(50)
```

## Step 2
- go left
```blocks
maqueen.motorRun(maqueen.Motors.M1, maqueen.Dir.CCW, 100)
maqueen.motorRun(maqueen.Motors.M2, maqueen.Dir.CW, 100)
basic.pause(300)
maqueen.motorStop(maqueen.Motors.All)
basic.pause(50)
```

## Step 3
- go right
```blocks
maqueen.motorRun(maqueen.Motors.M1, maqueen.Dir.CW, 100)
maqueen.motorRun(maqueen.Motors.M2, maqueen.Dir.CCW, 100)
basic.pause(300)
maqueen.motorStop(maqueen.Motors.All)
basic.pause(50)
```

## Step 4

Upload the program on Rotoy and see if you can complete the maze!

Once Rotoy can complete the maze, go to the next step!

## Step 5

Seems like your program grew quite a lot and you had to repeat the same moves!
That's where the functions come in.

## Step 6 @showhint

A function is a block of code that contains other instructions.

Look at this example:

To make Rotoy go straight by 1 move on the maze, you have to use all this code:
```blocks
maqueen.motorRun(maqueen.Motors.All, maqueen.Dir.CW, 100)
basic.pause(400)
maqueen.motorStop(maqueen.Motors.All)
basic.pause(50)
```

But if we put it in function called ``||functions:goStraight||``, then, we can simply just put:
```blocks
function goStraight () {
    maqueen.motorRun(maqueen.Motors.All, maqueen.Dir.CW, 100)
    basic.pause(400)
    maqueen.motorStop(maqueen.Motors.All)
    basic.pause(50)
}
goStraight()
```

## Step 7

Now, create 2 more functions - to ``||functions:turnLeft||`` and ``||functions:turnRight||``

## Step 8 @showhint

Finally, replace your previous code with the functions to solve the maze.

Here are the first few lines:
```blocks
function goStraight () {
}
function turnLeft () {
}
function turnRight () {
}
goStraight()
goStraight()
turnLeft ()
goStraight()
```

## Step 9

Test your code!