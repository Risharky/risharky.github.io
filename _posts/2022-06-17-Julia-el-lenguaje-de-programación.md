---
layout: post
title: Julia el lenguaje de programación
date: 2022-06-17 13:00
author: Ricardo Rodriguez Otero
comments: true
categories: [GIS, Julia]

---

[Julia](https://julialang.org/) es un lenguaje de programación creado en 2012 es relativamente joven a comparación de otros lenguajes de programación multi paradigma o multi propósito este en teoría es posible crear aplicaciones de escritorio, aplicaciones web entre otras cosas, está teniendo un interesante desarrollo en el campo de la ciencia y análisis de datos.

En datos tiene dos framework bastantes interesantes uno es [Flux.jl]([GitHub - FluxML/Flux.jl: Relax! Flux is the ML library that doesn&#39;t make you tensor](https://github.com/FluxML/Flux.jl))  para machine learning y para data science (similar a pandas o algunas funciones o paquetes de R)  [Dataframes.jl]([GitHub - JuliaData/DataFrames.jl: In-memory tabular data in Julia](https://github.com/JuliaData/DataFrames.jl)) , entre otros paquetes tambien tiene muchas opciones de visualización.

 A diferencia de python este lenguaje está orientado al rendimiento es mucho más rápido y eficiente que python, dado que Julia no es interpretado sino que compila usando el compilador **just-in-time (JIT)**, además de que es mucho más sencillo el manejo de datos en paralelo que con python o R.

En fin porque menciono Julia y no cosas relacionadas con Python, el ecosistema de python está madurando bien en muchos aspectos y es posible hacer todo con python, pero al manejar grandes volúmenes de datos ya python deja de ser una opcion para todo se hace necesario complementar procesos con lenguajes más rápidos como SQL, lo cual hace necesario aprender un segundo lenguaje, la combinación más popular es python+ R y SQL, pero R tiene una curva de aprendizaje complicada y sin contar que los paquetes de R dependiendo del ambiente funcionan o no.

R tiene un, pero en relación a su rendimiento para algunas cosas tiene la velocidad “suficiente” pero no tiene el rendimiento deseado por lo cual R a pesar de que tiene muchos paquetes, en mi caso empecé a ver otras opciones como SCALA o retomar JAVA que es similar a SCALA y funciona muy bien o C# que es un lenguaje que también multi propósito a diferencia de R que está orientado a estadística.

La necesidad de crear interfaces de formularios o una forma de publicar los resultados o la necesidad de desarrollar aplicaciones más complejas para el análisis de datos se puede cubrir con los lenguajes ya mencionados, que hace interesante a Julia para esto que tiene interoperabilidad permitiendo llamar funciones o programas hechos en python o R, incluso cosas de C++ java, también por su sintaxis similar a python es fácil de aprender y permite la rescritura de [algoritmos]([Replacing legacy code with Julia - Julia Community](https://forem.julialang.org/petrkryslucsd/replacing-legacy-code-with-julia-52ff)) hechos en lenguajes ya más maduros como Lisp o Fortran.

En adición a lo anterior tambien tiene el paradigma o la opción de [metaprogramación]([Metaprogramming · The Julia Language](https://docs.julialang.org/en/v1/manual/metaprogramming/)) lo cual permite llamar programas con mucha facilidad y le da mucha más compatibilidad en cosas desarrolladas en Julia u otros lenguajes . 

 Considero que en un futuro puede llegar a ser una buena competencia para python y R en el ecosistema de datos e incluso en otros como el desarrollo web, pero le puede jugar en contra que todavía no es tan conocido y se le considera un lenguaje de programación "raro" o muy reciente, lo estoy aprendiendo y lo que he visto me ha gustado incluso mucho más que con python y pensaría que es posible trabajar únicamente con Julia para resolver la mayoría de problemas en datos y gis(sí también tiene cosas interesantes en gis).

Para  aprender Julia estoy usando los mismos recursos que ofrecen los creadores y mantenedores del mismo, como [Julia Academy ]([JuliaAcademy](https://juliaacademy.com/courses)) o haciendo mini proyectos con [ejemplos]([Julia on Exercism](https://exercism.io/tracks/julia)) y por ultimo el canal de [youtube oficial]([The Julia Programming Language - YouTube](https://www.youtube.com/user/JuliaLanguage/playlists)) todos de acceso gratuito. 

Eso es todo, por ahora. 
