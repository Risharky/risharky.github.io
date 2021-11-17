---
layout: post
title: Calcular Identificador o contador de elementos en un Shapefile en ArcGIS
date: 2017-05-19 20:42
author: risharky
comments: true
categories: [ArcGIS, Python, Python Scripting, Tutoriales]
---
En algunas ocasiones se necesita crear shapefiles numerados en orden ya sea como un identificador u otro uso.

Para eso creamos en la tabla de atributos del archivo un nuevo campo como se ve en la imagen.

[caption id="attachment_181" align="aligncenter" width="260"]<img class=" size-full wp-image-181 aligncenter" src="/images/WP_media/2017/05/post.png" alt="post" width="260" height="110" /> Creando Campo adicional.[/caption]

Después de crear el campo, con el nombre que considere necesario en este caso será “id”, pero este campo debe ser creado con valores enteros,  se procede a calcular el id para eso, damos clic derecho sobre el encabezado o título del campo id y seleccionamos la opción de calculadora de campo como se ve en las imágenes.

[gallery ids="185,186" type="rectangular"]

En la calculadora de campo selección la opción de python en vez de la que está por defecto y  activa la opción de “Show Codeblock” y agregue el siguiente script:

[code language="python"]
counter = 0
def uniqueID():
 global counter
 counter += 1
return counter
[/code]

Después en el espacio “ID”  como se muestra en la imagen, agregue la siguiente opción:

[code language="python"]
uniqueID()
[/code]

&nbsp;

[gallery ids="190,191" type="rectangular"]

Este script se puede guardar para usarse las veces que considere necesario funciona en las versiones 10.x de Arcgis, en caso que desee iniciar en un numero diferente a 1, cambie el valor 1 en “counter” por el valor que desee que inicie el contador.

Como puede apreciar es algo muy sencillo y que puede guardar con la extensión *.cal

Espero que sea de ayuda.
