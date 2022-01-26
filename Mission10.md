# Mission10
```package
maqueen=github:dfrobot/pxt-maqueen
```

## Introduction @unplugged

This is it! Your final enemy!

## Step 1

You need to figure out by yourself how to make Rotoy sneek by Maybug!

Few hints:
- go slow (don't exceed speed of 100)
- you can turn each wheel with different speed (to make bigger circle)

```blocks
maqueen.motorRun(maqueen.Motors.M1, maqueen.Dir.CW, 50)
maqueen.motorRun(maqueen.Motors.M2, maqueen.Dir.CW, 100)
basic.pause(400)
maqueen.motorStop(maqueen.Motors.All)
basic.pause(50)
```

## Step 2

Good luck!