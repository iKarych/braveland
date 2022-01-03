# Mission 5
```package
maqueen=github:dfrobot/pxt-maqueen
```

## Introduction @unplugged

Now, it's time to learn new skills. Using Rotoy's ultrasonic sensor, you can measure how far away some objects are.

## Step 1

For this one, you will need these blocks:
- ``||maqueen:move||`` to start and stop motors,
- ``||maqueen:read ultrasonic sensor||`` to read the distance from Rotoy to the toad,
- ``||basic:show number||`` to display the distance to the toad,
- ``||logic:if else||`` to create logic when Rotoy should stop,
- ``||variable:distance||`` to store information from the sensor.

## Step 2 @showhint

First, check out how does the sensor work. Create the code below and put it on micro:bit:

```blocks
basic.forever(function () {
    basic.showNumber(maqueen.Ultrasonic(PingUnit.Centimeters))
})
```

Check if the value gets smaller when you move your hand closer to Rotoy's eyes or bigger when moving further.

## Step 3

Let's now do the same program, but let's keep information in a variable.
Variables can store information, for example we will use variable ``||variable:distance||`` to keep the distance (in cm) from Rotoy to the toad.

Follow the steps below:
1. Create new variable ``||variable:distance||``
2. ``||variable:set||`` it to read the number from the ultrasonic sensor
3. Display the value of the variable using ``||basic:show number||``

```blocks
let distance = 0
basic.forever(function () {
    distance = maqueen.Ultrasonic(PingUnit.Centimeters)
    basic.showNumber(distance)
})
```

Check if the value gets smaller when you move your hand closer to Rotoy's eyes or bigger when moving further.

## Step 4

The next step is to learn a little bit about ``||logic:if||`` statement.

Look at this example:
``||logic:if||`` I press button A, ``||logic:then||``
Rotoy will be happy,
``||logic:else||`` (or if not), then
Rotoy will be sad.

Try making this example in code and test it on micro:bit

```blocks
basic.forever(function () {
    if (input.buttonIsPressed(Button.A)) {
        basic.showIcon(IconNames.Happy)
    } else {
        basic.showIcon(IconNames.Sad)
    }
})
```

## Step 5

Finally, you are ready to combine all the new stuff that you've learned.

1. Create ``||variable:distance||`` and ``||variable:set||`` it to store information from the ultrasonic sensor.
2. Create ``||logic:if||`` statement that checks if ``||variable:distance||`` is bigger than 10 cm, ``||logic:then||`` allow Rotoy to slowly move forward.
3. Otherwise, ``||logic:else||``, make Rotoy stop.

```blocks
let distance = 0
basic.forever(function () {
    distance = maqueen.Ultrasonic(PingUnit.Centimeters)
    if (distance > 10) {
        maqueen.motorRun(maqueen.Motors.All, maqueen.Dir.CW, 50)
    } else {
        maqueen.motorStop(maqueen.Motors.All)
    }
})
```

## Step 6

Now, put the code on micro:bit and place the toad in front of it.

Your task is to make Rotoy stop 10 cm from the ugly toad! Good luck!