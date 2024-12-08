```package
roversa=github:eb8ga/pxt-roversa-2
```




# Roversa - Logic




## Introduction @showdialog




In this tutorial we will explore how logic statements give Roversa its "intelligence."




## Step 1: Conditional




A conditional statement, also known as an if-then statement, allows us to represent decision making through code.




From the ``||logic:Logic||`` category, select the ``||logic:if-then-else||`` block.




```blocks
basic.forever(function () {
   if (true) {
      
   }
})
```




## Step 2: Comparison


Comparison (greater than, less than and equal to) and Boolean (and, or, not) expressions are often used in conditional statements.


From the ``||logic:Logic||`` category, select the ``||logic:less than|`` **Comparison** block.


```blocks
basic.forever(function () {
   if (0 < 0) {
      
   }
})
```




## Step 3: Sensors


Logic statements are often used with sensors.


From the ``||input:Input||`` category, select ``||input:light level|`` block.




```blocks
basic.forever(function () {
   if (input.lightLevel() < 0) {
      
   }
})
```


## Step 4: Output




From the ``||basic:Basic||`` category, select two ``||basic:show icon||`` blocks.
From the ``||roversa:Roversa||`` extension, select the **drive** ``||roversa:forward||`` and  ``||roversa:stop||`` blocks.




```blocks
basic:showicon()
roversa.forward()
roversa.stop()


```




## Step 4: Code and Test Roversa




Now that you have the logic, comparison, sensor and output blocks, you are ready to code Roversa (click lightbulb icon for Hint).




``|Download|`` to transfer your code to Roversa.




```blocks
basic.forever(function () {
   if (input.lightLevel() < 30) {
       basic.showIcon(IconNames.Yes)
       roversa.forward()
   } else {
       basic.showIcon(IconNames.No)
       roversa.stop()
   }
})
```

