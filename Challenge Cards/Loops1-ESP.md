```package
roversa=github:eb8ga/pxt-roversa-2
```


# Roversa - Loops:Repeat


## Introduction @showdialog


En este tutorial exploramos el uso del bucle de repetición para hacer que Roversa se mueva en el cuadrado. 


## Step 1: Repeat


Los bucles son realmente útiles para repetir patrones. 


From ``||loops:bucles||`` category, select ``||loops:repetir [4] veces ejecutar||`` block.


```blocks
basic.forever(function () {
   // @highlight
   for (let index = 0; index < 4; index++) {
          
   }
})
```


## Step 2: Button Input


Desde el  ``||roversa:Roversa||`` extension, select the Roversa button ``||roversa:roversa en [Play]||`` bloque.


```blocks
roversa.onEvent()
```


## Step 3: Servo Output


Desde ``||roversa:Roversa||`` extension, select the ``||roversa:adelante||`` and ``||roversa:girar a la derecha|`` bloque.


```blocks
roversa.forward()
roversa.right()
```


## Step 4: Code and Test Roversa
Ahora que tiene los bloques de entrada y salida, esta listo para codificar a Roversa para que se mueva en un patron cuadrado  (haga clic en la bombilla para obtener una pista).


``|Download|`` para transferir su codigo a Roversa.


```blocks
roversa.onEvent(RoversaPin.P5, RoversaEvent.Click, function () {
    for (let index = 0; index < 4; index++) {
        roversa.forward()
        roversa.right()
    }
})
```





