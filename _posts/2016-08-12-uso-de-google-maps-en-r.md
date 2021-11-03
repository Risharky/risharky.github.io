---
layout: post
title: Uso de Google Maps en R
date: 2016-08-12 20:34
author: risharky
comments: true
categories: [Google Maps, mapa, R, Tutoriales, Unigis, WebMapping]
---
Google Maps actualmente es una herramienta que puede ser complementaria a muchas aplicaciones por los servicios y opciones de cartografía que ofrece google, por lo que se puede ahorrar dinero en proyectos muy pequeños o personales y tiempo para generar cosas básicas con cartografía temática y si combinamos esto con la potencia y versatilidad del lenguaje de programación R se pueden tener muy buenos resultados, en proyectos que requieran datos estadísticos o localización de los mismos, como en el siguiente ejemplo de mapa usando la librería de R Rgooglemaps.

[code language="r"]
#creando mapa de puntos con googlemaps
#se instala paquete de google maps para R, el cual carga desde internet información google
install.packages(&quot;RgoogleMaps&quot;)
#Se define espacio de trabajo
setwd(&quot;La ruta de la carpeta que defina&quot;)
#llamando librerias requeridas
require(RgoogleMaps)
library(maptools)
#leyendo datos
datos&lt;- readShapePoints(&quot;wgs84.shp&quot;)
#definiendo centro del mapa
lat = c(min(datos$Latitud),max(datos$Latitud));
lon = c(min(datos$Longitud),max(datos$Longitud));
#graficando mapa y puntos , es posible escoger mas opciones de mapa s escoge esta para una mejor compocision
MyMap&lt;- GetMap.bbox(latR =lat ,lonR = lon, maptype='terrain', destfile = &quot;garbage_locations.png&quot;);
pic = PlotOnStaticMap(MyMap)
# convirtiendo coordenadas georaficas a coordenadas de imagen
cord = LatLon2XY.centered(MyMap,datos$Latitud,datos$Longitud)
# coordenadas de sitios
points(cord$newX,cord$newY,col=colors()[4],lwd=1)
# ubicación de etiquetas
text(cord$newX,cord$newY,datos$Estacion,cex=0.8,col=colors()[4])
# Ajuste de coordendas de etiquetas para evitar traslape
loc_x = datos$Longitud; loc_y = datos$Latitud-0.005;
i_Canaveralejo = which(datos$Estacion==&quot;CaÃ±averalejo&quot;)
i_La_Ermita = which(datos$Estacion==&quot;La Ermita&quot;)
i_Compartir = which(datos$Estacion==&quot;Compartir&quot;)
i_Univalle = which(datos$Estacion==&quot;Univalle&quot;)
i_Pance = which(datos$Estacion==&quot;Pance&quot;)
i_Base_Aerea = which(datos$Estacion==&quot;Base Aerea&quot;)
i_Era = which(datos$Estacion==&quot;Era&quot;)
i_La_Flora = which(datos$Estacion==&quot;La Flora&quot;)
loc_x[i_Canaveralejo] = loc_x[i_Canaveralejo]-0.009;
loc_x[i_La_Ermita] = loc_x[i_La_Ermita]-0.009;
loc_x[i_Compartir] = loc_x[i_Compartir]-0.009;
loc_x[i_Univalle] = loc_x[i_Univalle]+0.005;
loc_y[i_Pance] = loc_y[i_Pance]+0.010;
loc_x[i_Base_Aerea] = loc_x[i_Base_Aerea]+0.005;
loc_x[i_Era] = loc_x[i_Era]+0.005;
loc_x[i_La_Flora] = loc_x[i_La_Flora]+0.005;
# Redibujando el mapa
pic = PlotOnStaticMap(MyMap)
cord = LatLon2XY.centered(MyMap,datos$Latitud,datos$Longitud)
points(cord$newX,cord$newY,col=&quot;blue&quot;,lwd=2)
# Nuevamente coordenadas corregidas de las etiquetas
cord = LatLon2XY.centered(MyMap,loc_y,loc_x)
text(cord$newX,cord$newY,datos$Estacion,cex=0.9,col=&quot;black&quot; )
[/code]

<img class=" size-full wp-image-113 aligncenter" src="https://risharkygis.files.wordpress.com/2016/10/mapa.png" alt="mapa" width="277" height="345" />Este seria el resultado del codigo anterior.
<p style="text-align:justify;">Si desean saber más sobre esta librería pueden revisar esta dirección <a href="https://cran.r-project.org/web/packages/RgoogleMaps/index.html">https://cran.r-project.org/web/packages/RgoogleMaps/index.html</a> cuenta con la documentación principal de la librería y en caso de otro ejemplo pueden revisar este enlace <a href="https://www.r-bloggers.com/heatmap-of-toronto-traffic-signals-using-rgooglemaps/">https://www.r-bloggers.com/heatmap-of-toronto-traffic-signals-using-rgooglemaps/</a></p>
<p style="text-align:justify;">Está la opción de estadística espacial, usan el lenguaje de programación R, como elemento principal de enseñanza.</p>
<p style="text-align:justify;">Espero que sea de utilidad :)</p>
