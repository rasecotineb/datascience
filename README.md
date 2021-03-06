# Analytics Portfolio

<!-- TOC -->

 - [My DataScience Portfolio](#analytics-portfolio)
    - [1. Machine Learning](#1-machine-learning) 
    - [2. Data Visualization](#2-data-visualization)
    - [3. Time Series](#3-time-series)
    - [4. Data Mining](#4-data-mining)
    - [5. Sentiment Analysis](#5-sentiment-analysis)
    - [6. Exploratory Data Analysis](#6-exploratory-data-analysis)


<!-- /TOC -->

## 1. Machine Learning
El proyecto que se describe a continuación tiene por objetivo la predicción de una variable continua ***Importe Total Factura*** mediante el uso de diversos algoritmos de regresión en combinación con diferentes configuraciones de hiperparámetros.
Los principales algoritmos que se han utilizado son:
1. __Multiple linear regression__
2. __SVR regressor__
3. __Random Forest regressor__
4. __Ensemble Voting regressor__
5. __Gradient Boosting__
6. __ADABoost__
7. __XGBoost__
8. __Stacking Regressor__
9. __MLP Regressor__

En el siguiente gráfico se puede observar, comparativamente, los resultados de los diferentes algoritmos de ML  basado en el coeficiente de determinación (R2)

![alt text][resultados-ml]

[resultados-ml]: https://github.com/rasecotineb/datascience/blob/master/machine-learning/resultados-machine-learning.JPG "Resultados de algoritmos ML"

> El proyecto aborda todas la etapas de un proyecto de datascience: entendimiento de la necesidad del negocio, comprensión de los datos, preprocesamiento de datos, evaluación de algoritmos, evaluación de resultados


Visitar notebook de [machine learning](https://github.com/rasecotineb/datascience/blob/master/machine-learning/Analisis_de_datos_Regresion_lineal_Machine_Learning_II_.ipynb)



## 2. Data Visualization
Actualmente vengo trabajando en un par de iniciativas de visualización de datos:
El primero de ellos tiene que ver con el uso de ***Dash*** de *plotly*.
Y un segundo relacionado a visualización geo-espacial (GIS)

Muy aparte de lo mencionado anteriormente, he utilizado la librería de `IPYWidgets` para dotar de interactividad a los gráficos que se utilizan regularmente para el análisis exploratorio de datos: *heatmaps, boxplots, scatterplots, pairplots, etc*. De este modo, el usuario del negocio puede realizar un analisis dinámico y focalizado a través de controles como: *range slider, combobox, radiobutton, label, etc*. 

En la siguiente figura se puede observar que el usuario tiene disponible la opción de utilizar un slider para modificar el rango de la variable *Cuota C.U* y observar como los gráficos se van ajustando a su criterio de análisis de forma dinámica
![alt text][pairplot]

[pairplot]: https://github.com/rasecotineb/datascience/blob/master/data-visualization/pairplot.JPG "Pairplot"


Para el análisis dinámico de correlación con el apoyo visual de un *heatmap*, el usuario cuenta con 2 sliders: uno para la variable target *Importe Total Factura S/.* y el otro para   *Cuota C.U*
![alt text][heatmap]

[heatmap]: https://github.com/rasecotineb/datascience/blob/master/data-visualization/heatmap.JPG "Heatmap"

Para este último caso, el usuario cuenta con más opciones para el análisis dinámico de la distribución de las variables numéricas mediante el uso de *boxplots*: *combobox* para la selección de variables a analizar,  *slider* dinámico en función a la variable seleccionada en el *combobox*, *radiobutton* para descartar o no la presencia de outliers en los *boxplots*
![alt text][boxplot]

[boxplot]: https://github.com/rasecotineb/datascience/blob/master/data-visualization/boxplot.JPG "Boxplot"

Cada una de las gráficas anteriores se encuentran contenidas en diferentes *tabs* o *pestañas*, de esta manera el usuario tiene una visualización más ordenada de las opciones que tiene disponibles para iniciar su proceso exploratorio de datos, sin que la excesiva aparición de controles lo intimide.

>Tópicos: Geolocalizacion, Dashboard, Frontend, IPYWidgets, User interaction

## 3. Time Series
El análisis y modelado de series temporales viene captando el interés de las empresas que buscan optimizar sus predicciones en base a información histórica temporal como pueden ser sus ventas que, muchas veces, presentan estacionalidad.

En el siguiente gráfico se muestra la tendencia de búsquedas en *Google* sobre este tópico en los últimos 5 años
![alt text][time-series-trend]

[time-series-trend]: https://github.com/rasecotineb/datascience/blob/master/time-series/time-series-trend.JPG "Tendencia sobre interés en series temporales durante los últimos 5 años "

A continuación muestro algunos de los modelos que he venido trabajando en analisis de series temporales
### Análisis Univariado
1. **ARIMA**

Presentación del modelo autoregresivo integrado con medias móviles.

Visitar notebook de [ARIMA](https://github.com/rasecotineb/datascience/blob/master/time-series/ModeloARIMA.ipynb)

2. **SARIMA**

Presentación de la generalización del modelo ARIMA con el componente estacional

Visitar notebook de [SARIMA](https://github.com/rasecotineb/datascience/blob/master/time-series/ModeloSARIMA.ipynb)

### Análisis Multivariado
1. **VAR**

Presentación del modelo autoregresivo con más de una serie temporal.

Visitar notebook de [VAR](https://github.com/rasecotineb/datascience/blob/master/time-series/ModeloVAR.ipynb)


>Tópicos: Stationarity, Seasonality, ADF, Log transformation, Box-cox transformation, Autocorrelation, Partial Autocorrelation
## 4. Data Mining
Resulta útil, sobre en todo en negocios con una alta transaccionalidad comercial como el caso de los retailers, la posibilidad de poder identificar patrones, por ejemplo, artículos que tienen una alta frecuencia de rotación conjunta. Esta información resulta en importantes insights para determinar los patrones de compra de los clientes y en base a ello diseñar, por ejemplo, estrategias de ventas cruzadas o publicidad focalizada en parte del portafolio de productos.
### Problem Statement
Se cuenta con una empresa de consumo masivo que desea identificar patrones de consumo a partir de la data transaccional de las ventas a sus clientes. A partir de esta iniciativa podrá identificar cuáles son las combinaciones de productos con mayor frecuencia de venta y como se afecta la compra de un producto en función a otros. 

La siguiente gráfica muestra la solución al problema planteado: se identifica claramente patrones de consumo con un nivel de certeza específico y con un umbral de frecuencia relevante mínimo.
La primera línea del cuadro se puede interpretar de la siguiente manera: *Todos aquellos clientes que compran el item 7 han comprado también el item 20 con una frecuencia de 9 veces y con un nivel de confianza de 81.82%, es decir que esas 9 veces del patrón 7->20, corresponde al 81.82% de todas las compras del item 7*

![alt text][insigths]

[insigths]: https://github.com/rasecotineb/datascience/blob/master/datamining/association-rules.JPG "Reglas de asociación - Patrones de consumo"
Visitar notebook de [datamining](https://github.com/rasecotineb/datascience/blob/master/datamining/Itemset_Pattern.ipynb)
>Tópicos: Data pattern, insights, itemsets, association rules

## 5. Sentiment Analysis
### Problem Statement
A finales del mes de Junio, a raiz de la crisis sanitaria producto del COVID-19, se cuestionó que las clínicas privadas en Perú cobraban exorbitantes sumas por el tratamiento de pacientes infectados por el COVID-19 y que no tenían seguro privado. Ante esto el gobierno del Perú dio un ultimatum a las clínicas para llegar un acuerdo sobre las tarifas solidarias a cobrar por el tratamiento de pacientes con COVID-19. Ante esto se plantea conocer la percepción de la gente, su posición acerca de los anuncios dados por el gobierno sin necesidad de esperar una encuesta que tomaría más tiempo y recursos.



En la siguiente gráfica se puede apreciar la nube de palabras predominantes en twitter sobre el acuerdo del gobierno con las clínicas privadas durante la crisis del COVID-19.


![alt text][main-words]

[main-words]: https://github.com/rasecotineb/datascience/blob/master/sentiment-analysis/main-words-pos.JPG "Nube de palabras"

La curva ROC que se muestra a continuación muestra la relacion entre la tasa de *verdaderos positivos (TPR)* y *falsos positivos (FPR)* y la performance del modelo de clasificación para diferentes valores de *thresholds*.

![alt text][roc-curve]

[roc-curve]: https://github.com/rasecotineb/datascience/blob/master/sentiment-analysis/roc-curve-sentyment-analysis.JPG "Curva ROC"

Visitar notebook de [sentiment analysis](https://github.com/rasecotineb/datascience/blob/master/sentiment-analysis/Twitter_Analisis_de_Sentimientos.ipynb)

>Tópicos: NLP, Bag of words, TFIDF, API Twitter, Naive Bayes, Logistic Regression
## 6. Exploratory Data Analysis
En análisis exploratorio de datos que se muestra a continuación se basa en el análisis descriptivo de la información de un dataset que permita el mayor entendimiento posible sobre la data mediante el uso de elementos gráficos como: *diagrama de barras, boxplot, heatmaps, entre otros*

![alt text][box-hist]

[box-hist]: https://github.com/rasecotineb/datascience/blob/master/eda/EDA1.JPG "Boxplot + Histograma"




![alt text][bar]

[bar]: https://github.com/rasecotineb/datascience/blob/master/eda/EDA2.JPG "Diagrama de barras"




![alt text][bar-stacked]

[bar-stacked]: https://github.com/rasecotineb/datascience/blob/master/eda/EDA4.JPG "Diagrama de barras - Stack"




![alt text][correlacion]

[correlacion]: https://github.com/rasecotineb/datascience/blob/master/eda/EDA3.JPG "Correlacion de variables"

>Tópicos: Plotting, Boxplot, Correlation, R
