```package
roversa=github:eb8ga/pxt-roversa-2
```


# Roversa - Input/Output


## Introduction @showdialog


In this tutorial we will explore input and output with Roversa.


## Step 1: Button Input


Input is information we put into the robot like pressing buttons or using sensors.


From the ``||roversa:Roversa||`` extension, select the Roversa button ``||roversa:Roversa button on||`` block.


```blocks
roversa.onEvent()
```


## Step 2: Servo Output


Output is something that comes out of Roversa like the LEDs lighting up  or the
servos turning the wheels.


From the ``||roversa:Roversa||`` extension, select the **drive** ``||roversa:forward||`` and  **drive** ``||roversa:backward||`` blocks.


```blocks
roversa.forward()
roversa.backward()
```


## Step 3: LED Output


From the ``||basic:Basic|`` category, select two ``||basic:show icon||`` blocks.


```blocks
basic.showIcon(IconNames.Triangle)
```


## Step 4: Code and Test Roversa


Now that you have the input and output blocks, you are ready to recode one of the buttons on Roversa (click lightbulb icon for Hint).


``|Download|`` to transfer your code to Roversa.


```blocks
roversa.onEvent(RoversaPin.P5, RoversaEvent.Click, function () {
    roversa.forward()
    basic.showIcon(IconNames.Triangle)
    roversa.backward()
    basic.showIcon(IconNames.Cow)
})
```





