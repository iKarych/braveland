# Mission 7
```package
maqueen=github:dfrobot/pxt-maqueen
```

## Introduction @unplugged

You managed to stop in front of the toad but now... it wants to jump on you!

## Step 1

Use Rotoy's movement blocks:

```blocks
maqueen.motorRun(maqueen.Motors.M1, maqueen.Dir.CW, 255)
maqueen.motorRun(maqueen.Motors.M2, maqueen.Dir.CCW, 255)
basic.pause(200)
maqueen.motorStop(maqueen.Motors.All)
```