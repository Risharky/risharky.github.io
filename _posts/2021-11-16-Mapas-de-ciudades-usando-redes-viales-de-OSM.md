---
layout: post
title: Mapas de ciudades usando redes viales de OSM
date: 2020-10-16 20:28
author: risharky
comments: true
categories: [GIS, python]

---

El paquete para python OSMnx permite descargar redes viales de OSM y graficarlos con diferentes configuraciones, este paquete  tiene 2 opciones de crear mapas, una definiendo la ciudad y el país , la otra funciona adicionando a la ciudad un punto central y un radio especifico, es una forma de crear mapas sencillos y rápidos tal vez para representar áreas de estudio en informes o documentos, pero la capa como tal es pesada por lo que el procesamiento dependiendo de la ciudad puede demorar de unos segundos a minutos, si se descarga la ciudad completa.

![mapaOSMnx](/images/mapaOSMnx.png)

 Por ejemplo la imagen corresponde a las vías de Bogotá-Colombia el código del notebook esta en el [enlace](https://github.com/Risharky/Mapas_python/blob/main/Notebooks/mapas%20con%20OSMnx.ipynb), como fuentes se usar las siguientes referencias [1](https://towardsdatascience.com/creating-beautiful-maps-with-python-6e1aae54c55c) y [2](https://osmnx.readthedocs.io/en/stable/)
