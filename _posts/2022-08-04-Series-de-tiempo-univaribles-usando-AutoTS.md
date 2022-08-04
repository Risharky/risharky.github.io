---
layout: post
title: Series de tiempo univaribles usando Auto TS
date: 2022-06-17 11:00
author: Ricardo Rodriguez Otero
comments: true
categories: [Forecast, Python]

---

Las series de tiempo permiten graficar o modelar datos en secuencias temporales con diferentes tipos de periocidad temporal o lo ideal es que los datos tengan la misma “escala temporal”. 


La librería de Python [AutoTS](https://github.com/winedarksea/AutoTS) permite usar datos de series de tiempo univarible(uno sola variable) para hacer predicciones o previsiones usando datos pasados de la variable a predecir es bastante sencilla de usar sus usos pueden ser múltiples, la librería usa varios paquetes como statsmodels, prophet, sklearn, pytorch-forecasting entre otros, según la periocidad de los datos deberá analizar que modelo se ajusta mejor a sus datos. 


Elabore un [dashboard](https://risharky-forecaster-experiment-main-vv9dtz.streamlitapp.com/) (podra verlo en el enlace) con la librería streamlit con datos diarios con el precio del dólar en Colombia en donde uso 3 modelos [ARIMA](https://es.wikipedia.org/wiki/Modelo_autorregresivo_integrado_de_media_m%C3%B3vil) (Auto Regressive Integrated Moving Average), [GLM](https://en.wikipedia.org/wiki/Generalized_linear_model) (generalized linear model) y [Theta](https://www.statsmodels.org/devel/examples/notebooks/generated/theta-model.html) que son modelos de la librería statsmodels, en donde se puede ver la diferencia entre las prediciones de cada modelo, siendo el modelo ARIMA el mas “preciso” esto se hace a modo de experimento.

 Los datos usados son datos reales del precio del dólar pero las predicciones son eso prediciones, que pueden ser usadas para la toma de algún tipo de decisión, en este caso creo que puede ser útil para identificar modelos y ya trabajar con estos con sus versiones multivariadas o análisis de varias variables de forma que se pueda tomar decisiones más acertadas, en temas comerciales o financieros en el caso que se use para divisas o ventas, también se podría usar para hacer predicciones de variables ambientales entre otros .
