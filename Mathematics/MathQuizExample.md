```package
roversa=github:eb8ga/pxt-roversa-2
```




# Roversa - Comparison Math Quiz




## Introduction @showdialog




In this tutorial we will explore how to create a robot math quiz on comparisons.


## Step 1: Conditional




A conditional statement, also known as an if-then statement, allows us to represent decision making through code.




From the ``||logic:Logic||`` category, select the ``||logic:if-then-else||`` block.




```blocks
basic.forever(function () {
   if (true) {
      
   } else {
      
   }
})
```




## Step 2: Comparison


Comparison (greater than, less than and equal to) are often used in conditional statements.


From the ``||logic:Logic||`` category, select the ``||logic:less than|`` **Comparison** block and change to **greater than** symbol.


```blocks
basic.forever(function () {
   if (0 > 0) {
      
   }
})
```




## Step 3: Math


Computing devices excel at math because they can solve math problems so fast.


From the ``||math:Math||`` category, select two ``||math: 0 / 0|`` blocks. Use these blocks to represent two different fractions, for instance 7/8 and 2/3.


## Step 4: Input


For the math quiz, you can check your answer to the comparison by pressing this key.


From the ``||roversa:Roversa||`` extension, select the ``||roversa:Roversa button on||`` block.




## Step 5: Output


You will show the answer to the comparison math quiz by creating greater than and less than symbols for the LEDs and having Roversa turn towards the value that is greater.




From the ``||basic:Basic||`` category, select two ``||basic:show leds||`` blocks. Make one a **greater than** symbol and one a **lesser than** symbol.


From the ``||roversa:Roversa||`` extension, select the **drive** ``||roversa:right||`` and  ``||roversa:left||`` blocks.




```blocks
basic:showLeds()
roversa.right()
roversa.left()


```




## Step 6: Code and Test Roversa




Now that you have the logic, comparison, input and output blocks, you are ready to code Roversa to create a math quiz (click lightbulb icon for Hint).




``|Download|`` to transfer your code to Roversa.




```blocks
roversa.onEvent(RoversaPin.P5, RoversaEvent.Click, function () {
   if (7 / 8 > 2 / 3) {
       basic.showLeds(`
           . . # . .
           . . . # .
           . . . . #
           . . . # .
           . . # . .
           `)
       roversa.left()
   } else {
       basic.showLeds(`
           . . # . .
           . # . . .
           # . . . .
           . # . . .
           . . # . .
           `)
       roversa.right()
   }
})
basic.forever(function () {
  
})


```



