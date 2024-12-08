```package
roversa=github:eb8ga/pxt-roversa-2
```


# Roversa - Loops:Forever and While


## Introduction @showdialog


En este tutorial exploramos el uso de los bucles eterno y para que Roversa enciende la pantalla LED mientras presionas el botón. 




## Step 1: Repeat


El bucle eterno es útil si desea verificar que una condición sea verdadera durante la vida útil del programa. El bucle mientras es util si desea repetir un patron basandose en una condicion en lugar de varias veces.


From ``||loops:bucles||`` category, select ``||loops:mientras [falso] ejecutar||`` block. Update from false to true.


```blocks
basic.forever(function () {
   while (true {
      
   }
})
```


## Step 2: Button Input


From the ``||roversa:Roversa||`` extension, select the Roversa button ``||roversa:roversa [Play] es presionado||`` block.


```blocks
basic.forever(function () {
   while (roversa.isPressed(RoversaPin.P8)) {
      
   }
})
```


## Step 3: LED Output


From the ``||basic:Basic|`` category, select ``||basic:mostrar icono||`` and ``||basic:borrar la pantalla||`` blocks.


```blocks
basic.showIcon(IconNames.Triangle)
basic.clearScreen()
```


## Step 4: Code and Test Roversa


Ahora que tiene el bucle en los bloques de entrada y salida, estas listo para codificar Roversa para que enciendan los LED cuando se presiona un botón (haga clic en el icono de la bombilla para obtener una pista). 


``|Download|`` to transfer your code to Roversa.


```blocks
basic.forever(function () {
   while (roversa.isPressed(RoversaPin.P8)) {
       basic.showIcon(IconNames.Ghost)
   }
   basic.clearScreen()
})
```





