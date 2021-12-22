# Mission 6
```package
maqueen=github:dfrobot/pxt-maqueen
```

## Introduction @unplugged

You managed to stop in front of the toad but now... it wants to jump on you!

## Step 1 @showhint

You are going to continue where you finished last time:

```blocks
let distance = 0
basic.forever(function () {
    distance = maqueen.Ultrasonic(PingUnit.Centimeters)
    basic.showNumber(distance)
    if (distance > 10) {
        maqueen.motorRun(maqueen.Motors.All, maqueen.Dir.CW, 50)
    } else {
        maqueen.motorStop(maqueen.Motors.All)
    }
})
```


## Step 2

Now, after Rotoy stops, you must make it turn around (180 degrees) and drive far away as fast as possible.

Make sure to test how long pause do you need so that Rotoy turns around exactly by 180 degrees!

```blocks
maqueen.motorRun(maqueen.Motors.M1, maqueen.Dir.CW, 100)
maqueen.motorRun(maqueen.Motors.M2, maqueen.Dir.CCW, 100)
basic.pause(200)
maqueen.motorRun(maqueen.Motors.All, maqueen.Dir.CW, 255)
basic.pause(5000)
maqueen.motorStop(maqueen.Motors.All)
```

## Step 3

Good luck on your mission!
```