# Mission 4
```package
maqueen=github:dfrobot/pxt-maqueen
```

## Introduction @unplugged

Good job on the previous one! Now, let's figure out how to make Rotoy move

## Step 1

For this one, you will need to blocks:
- ``||maqueen:move||`` to start and stop motors,
- ``||basic:pause||`` to set how long motors should run.

## Step 2 @showhint

Check this out! In this example, this will happen:
1. Both motors are turned on - Rotoy goes straight
2. Rotoy will go straight for 1000 ms (or 1 second)
3. Rotoy will stop - both motors are set to 0

```blocks
maqueen.motorRun(maqueen.Motors.All, maqueen.Dir.CW, 100)
basic.pause(1000)
maqueen.motorRun(maqueen.Motors.All, maqueen.Dir.CW, 0)
```

## Step 3 @showhint

To turn right you can use these blocks

```blocks
maqueen.motorRun(maqueen.Motors.M1, maqueen.Dir.CW, 100)
maqueen.motorRun(maqueen.Motors.M2, maqueen.Dir.CCW, 100)
basic.pause(300)
```

## Step 4 @showhint

And left

```blocks
maqueen.motorRun(maqueen.Motors.M1, maqueen.Dir.CCW, 100)
maqueen.motorRun(maqueen.Motors.M2, maqueen.Dir.CW, 100)
basic.pause(300)
```

## Step 5

Now, with all that knowledge, make Rotoy move in square!

## Step 6

Click ``|Download|`` to transfer your code to micro:bit!