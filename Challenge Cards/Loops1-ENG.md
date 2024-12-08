```package
roversa=github:eb8ga/pxt-roversa-2
```


# Roversa - Loops:Repeat


## Introduction @showdialog


In this tutorial we will explore using the repeat loop to get Roversa moving in a square.


## Step 1: Repeat


Loops are really useful for repeating patterns.


From ``||loops:Loops||`` category, select ``||loops:repeat [4] times||`` block


```blocks
basic.forever(function () {
   // @highlight
   for (let index = 0; index < 4; index++) {
          
   }
})
```


## Step 2: Button Input


From the ``||roversa:Roversa||`` extension, select the Roversa button ``||roversa:Roversa button on||`` block.


```blocks
roversa.onEvent()
```


## Step 3: Servo Output


From the ``||roversa:Roversa||`` extension, select the **drive** ``||roversa:forward||`` and  **turn** ``||roversa:right|`` blocks.


```blocks
roversa.forward()
roversa.right()
```


## Step 4: Code and Test Roversa


Now that you have the input and output blocks, you are ready to code Roversa to move in a square pattern (click lightbulb icon for Hint).


``|Download|`` to transfer your code to Roversa.


```blocks
roversa.onEvent(RoversaPin.P5, RoversaEvent.Click, function () {
    for (let index = 0; index < 4; index++) {
        roversa.forward()
        roversa.right()
    }
})
```





