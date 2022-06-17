---

layout: post
title: Que es RSurvey y como funciona?
date: 2020-10-16 20:28
author: risharky
comments: true
categories: [GIS, R]

---

<!-- wp:jetpack/markdown {"source":"\n\nRSurvey es un paquete desarrollado para R por el servicio geol\u00f3gico de estados unidos, este paquete permite importar datos espaciales en diferentes formatos, como shapefile, datos desde archivos Excel o textos entre otros, lo particular de este paquete es que cuenta con interfaz grafica - GUI . \n\npara varios usuarios puede ser de ayuda en R o en algunos casos puede interferir ya que consume memoria RAM.\n\npara instalar este paquete use la siguiente instrucci\u00f3n:\n\n`install.packages(\u0022RSurvey\u0022)`\n\nEn caso que este usando Rstudio de clic en tools install packages y digite \u0022RSurvey\u0022.\n\nDespu\u00e9s de instalado digite la siguiente:\n\n`library(RSurvey)`\n\nTenga en cuenta que en caso de consultar la ayuda de alguna de las herramientas del paquete desde el GUI, esta se desplegara en rstudio o en el IDE que este usando en su momento, no se abrir\u00e1 una nueva venta como si pasa con los gr\u00e1ficos 3D.\n\nLA interfaz gr\u00e1fica es muy sencilla esta compuesta de 5 men\u00fas principales como se muestra a continuaci\u00f3n \n\n"} -->

<div class="wp-block-jetpack-markdown"><p>RSurvey es un paquete desarrollado para R por el servicio geológico de estados unidos, este paquete permite importar datos espaciales en diferentes formatos, como shapefile, datos desde archivos Excel o textos entre otros, lo particular de este paquete es que cuenta con interfaz grafica - GUI .</p>
<p>para varios usuarios puede ser de ayuda en R o en algunos casos puede interferir ya que consume memoria RAM.</p>
<p>para instalar este paquete use la siguiente instrucción:</p>
<p><code>install.packages("RSurvey")</code></p>
<p>En caso que este usando Rstudio de clic en tools install packages y digite "RSurvey".</p>
<p>Después de instalado digite la siguiente:</p>
<p><code>library(RSurvey)</code></p>
<p>Tenga en cuenta que en caso de consultar la ayuda de alguna de las herramientas del paquete desde el GUI, esta se desplegara en rstudio o en el IDE que este usando en su momento, no se abrirá una nueva venta como si pasa con los gráficos 3D.</p>
<p>LA interfaz gráfica es muy sencilla esta compuesta de 5 menús principales como se muestra a continuación</p>
</div>
<!-- /wp:jetpack/markdown -->

<!-- wp:image {"align":"center","id":228,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/1.png"><img src="https://risharkygis.files.wordpress.com/2020/10/1.png?w=315" alt="" class="wp-image-228" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":229,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/2.png"><img src="https://risharkygis.files.wordpress.com/2020/10/2.png?w=292" alt="" class="wp-image-229" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":230,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/3.png"><img src="https://risharkygis.files.wordpress.com/2020/10/3.png?w=452" alt="" class="wp-image-230" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":231,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/4.png"><img src="https://risharkygis.files.wordpress.com/2020/10/4.png?w=400" alt="" class="wp-image-231" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":232,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/5.png"><img src="https://risharkygis.files.wordpress.com/2020/10/5.png?w=396" alt="" class="wp-image-232" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":233,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/6.png"><img src="https://risharkygis.files.wordpress.com/2020/10/6.png?w=384" alt="" class="wp-image-233" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":234,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/7.png"><img src="https://risharkygis.files.wordpress.com/2020/10/7.png?w=313" alt="" class="wp-image-234" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":235,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/8.png"><img src="https://risharkygis.files.wordpress.com/2020/10/8.png?w=384" alt="" class="wp-image-235" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:jetpack/markdown {"source":"A continuaci\u00f3n una peque\u00f1a prueba de la funcionalidad de este paquete, importe un set de datos de ejemplo de la librer\u00eda leaflet."} -->

<div class="wp-block-jetpack-markdown"><p>A continuación una pequeña prueba de la funcionalidad de este paquete, importe un set de datos de ejemplo de la librería leaflet.</p>
</div>
<!-- /wp:jetpack/markdown -->

<!-- wp:image {"align":"center","id":236,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/9.png"><img src="https://risharkygis.files.wordpress.com/2020/10/9.png?w=467" alt="" class="wp-image-236" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:jetpack/markdown {"source":"Usando el men\u00fa de variables o view  se puede acceder al \u0022Variable Manager\u0022(dar clic en el archivador), el cual le mostrara la informaci\u00f3n b\u00e1sica de cada uno de los atributos de la capa o set de datos. Puede editar algunas caracter\u00edsticas de cada una de las \u0022variables\u0022 o atributos desde esta ventana."} -->

<div class="wp-block-jetpack-markdown"><p>Usando el menú de variables o view  se puede acceder al "Variable Manager"(dar clic en el archivador), el cual le mostrara la información básica de cada uno de los atributos de la capa o set de datos. Puede editar algunas características de cada una de las "variables" o atributos desde esta ventana.</p>
</div>
<!-- /wp:jetpack/markdown -->

<!-- wp:image {"align":"center","id":237,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/10.png"><img src="https://risharkygis.files.wordpress.com/2020/10/10.png?w=726" alt="" class="wp-image-237" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:jetpack/markdown {"source":"En la ventana principal esta disponible la funci\u00f3n plot , el paquete autom\u00e1ticamente cargara las coordenadas(CRS WGS84, esto se puede editar o seleccionar usando la informaci\u00f3n de la librer\u00eda PROJ ), como se muestra en la imagen el eje z puede ser cualquier variable num\u00e9rica del set de datos, al seleccionar la opci\u00f3n de graficar superficie mas puntos, la superficie corresponde a la interpolaci\u00f3n de los datos Z, R desplegara una caja aparte con este gr\u00e1fico con clic derecho en el gr\u00e1fico lo puede exportar al formato deseado. "} -->

<div class="wp-block-jetpack-markdown"><p>En la ventana principal esta disponible la función plot , el paquete automáticamente cargara las coordenadas(CRS WGS84, esto se puede editar o seleccionar usando la información de la librería PROJ ), como se muestra en la imagen el eje z puede ser cualquier variable numérica del set de datos, al seleccionar la opción de graficar superficie mas puntos, la superficie corresponde a la interpolación de los datos Z, R desplegara una caja aparte con este gráfico con clic derecho en el gráfico lo puede exportar al formato deseado.</p>
</div>
<!-- /wp:jetpack/markdown -->

<!-- wp:image {"align":"center","id":238,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/11.png"><img src="https://risharkygis.files.wordpress.com/2020/10/11.png?w=337" alt="" class="wp-image-238" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:jetpack/markdown {"source":"En el men\u00fa plot encontrara muchas opciones para generar gr\u00e1ficos y de configuraci\u00f3n, permitiendo crear mapas muy sencillos con la informaci\u00f3n generada, como se muestra a continuaci\u00f3n. "} -->

<div class="wp-block-jetpack-markdown"><p>En el menú plot encontrara muchas opciones para generar gráficos y de configuración, permitiendo crear mapas muy sencillos con la información generada, como se muestra a continuación.</p>
</div>
<!-- /wp:jetpack/markdown -->

<!-- wp:image {"align":"center","id":240,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/13.png"><img src="https://risharkygis.files.wordpress.com/2020/10/13.png?w=605" alt="" class="wp-image-240" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":241,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/rplot.png"><img src="https://risharkygis.files.wordpress.com/2020/10/rplot.png?w=614" alt="" class="wp-image-241" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:image {"align":"center","id":242,"sizeSlug":"large","linkDestination":"media"} -->

<div class="wp-block-image"><figure class="aligncenter size-large"><a href="https://risharkygis.files.wordpress.com/2020/10/rplot01.png"><img src="https://risharkygis.files.wordpress.com/2020/10/rplot01.png?w=614" alt="" class="wp-image-242" /></a></figure></div>
<!-- /wp:image -->

<!-- wp:jetpack/markdown {"source":"Rsurvey es un paquete muy sencillo pero que puede facilitar importar informaci\u00f3n a R o Exportarla y realizar una exploraci\u00f3n b\u00e1sica de los datos a manipular, para mas informaci\u00f3n consultar [el manual de referencia](https:\/\/cran.r-project.org\/web\/packages\/RSurvey\/RSurvey.pdf ) o sus [vi\u00f1etas](https:\/\/cran.r-project.org\/web\/packages\/RSurvey\/index.html)  y para [mas informaci\u00f3n](https:\/\/www.r-project.org\/nosvn\/pandoc\/RSurvey.html ) "} -->

<div class="wp-block-jetpack-markdown"><p>Rsurvey es un paquete muy sencillo pero que puede facilitar importar información a R o Exportarla y realizar una exploración básica de los datos a manipular, para mas información consultar <a href="https://cran.r-project.org/web/packages/RSurvey/RSurvey.pdf">el manual de referencia</a> o sus <a href="https://cran.r-project.org/web/packages/RSurvey/index.html">viñetas</a>  y para <a href="https://www.r-project.org/nosvn/pandoc/RSurvey.html">mas información</a></p>
</div>
<!-- /wp:jetpack/markdown -->
