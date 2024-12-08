```package
roversa=github:eb8ga/pxt-roversa-2
```




# Roversa - Input/Output




## Introduction @showdialog


En este tutorial exploramos la entrada y salida con Roversa.




## Step 1: Button Input


La entrada es imformacion que ponemos en el robot, como presionar botones o usar sensores. 




From the ``||roversa:Roversa||`` extension, select the Roversa button ``||roversa:roversa en Play||`` block.


```blocks
roversa.onEvent()
```


## Step 2: Servo Output
La salida es algo que sale de Roversa, como los LED’s que se encienden o los servos que hacen girar las ruedas. 


From the ``||roversa:Roversa||`` extension, select the ``||roversa:adelante|`` and ``||roversa:retroceder|`` blocks.


```blocks
roversa.forward()
roversa.backward()
```


## Step 3: LED Output


From the ``||basic:básico|`` category, select two ``||baisc:monstrar icono||`` blocks.


```blocks
basic.showIcon(IconNames.Triangle)
```


## Step 4: Code and Test Roversa


Ahora que tiene los bloques de entrada y salida , esta listo para recodificar uno de los botones de Roversa (haga clic en el icono de bombilla para obtener una pista).


``|Download|`` to transfer your code to Roversa.


```blocks
roversa.onEvent(RoversaPin.P5, RoversaEvent.Click, function () {
   roversa.forward()
   basic.showIcon(IconNames.Triangle)
   roversa.backward()
   basic.showIcon(IconNames.Cow)
})
```


