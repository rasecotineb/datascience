# Analytics Portfolio

<!-- TOC -->

 - [My DataScience Portfolio](#analytics-portfolio)
    - [1. Machine Learning](#machine-learning)
    - [2. Data Visualization](#data-visualization)
    - [3. Time Series](#time-series)
    - [4. Data Mining](#data-mining)
    - [Sentiment Analysis](#sentiment-analysis)
    - [6. Exploratory Data Analysis](#exploratory-data-analysis)


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

1. __Name__: Nombre del videojuego.
+ _Variable_: Cualitativa
  + _MENSAJE_
+ _Tipo_: Nominal


## 2. Data Visualization
Actualmente vengo trabajando en un par de iniciativas de visualización de datos:
El primero de ellos tiene que ver con el uso de ***Dash*** de *plotly*.
Y un segundo relacionado a visualización geo-espacial

Muy aparte de lo mencionado anteriormente, he utilizado la librería de ```IPYWidgets``` para dotar de interactividad a los gráficos que se utilizan regularmente para el análisis exploratorio de datos: *heatmaps, boxplots, scatterplots, pairplots, etc*. De este modo, el usuario del negocio puede realizar un analisis dinámico y focalizado a través de controles como: *range slider, combobox, radiobutton, label, etc*. 
>Tópicos: Geolocalizacion, Dashboard, Frontend

## 3. Time Series
A continuación muestro algunos de los modelos que he venido trabajando en analisis de series temporales
### Analisis Univariado
1. **ARIMA**
2. **SARIMA**

### Analisis Multivariado
1. **VAR**
2. **VARMA**

>Tópicos: Stationarity, Seasonality, ADF, Log transformation, Box-cox transformation, Autocorrelation, Partial Autocorrelation
## 4. Data Mining
Resulta útil, sobre en todo en negocios con una alta transaccionalidad comercial como el caso de los retailers, la posibilidad de poder identificar patrones, por ejemplo, artículos que tienen una alta frecuencia de rotación conjunta. Esta información resulta en importantes insights para determinar los patrones de compra de los clientes y en base a ello diseñar, por ejemplo, estrategias de ventas cruzadas o publicidad focalizada en parte del portafolio de productos.
### Problem Statement
Se cuenta con una empresa de consumo masivo que desea identificar patrones de consumo a partir de la data transaccional de las ventas a sus clientes. A partir de esta iniciativa podrá identificar cuáles son las combinaciones de productos con mayor frecuencia de venta y como se afecta la compra de un producto en función a otros. 

La siguiente gráfica muestra la solución al problema planteado: se identifica claramente patrones de consumo con un nivel de certeza específico y con un umbral de frecuencia relevante mínimo.
La primera línea del cuadro se puede interpretar de la siguiente manera: *Todos aquellos cliente que compran el item 7 han comprado también el item 20 con una frecuencia de 9 veces y con un nivel de confianza de 81.82%, es decir que esas 9 veces del patrón 7->20, corresponde al 81.82% de todas las compras del item 7*

![alt text][insigths]

[insigths]: https://github.com/rasecotineb/datascience/blob/master/datamining/association-rules.JPG "Reglas de asociación - Patrones de consumo"
Visitar notebook de [datamining](https://github.com/rasecotineb/datascience/blob/master/datamining/Itemset_Pattern.ipynb)
>Tópicos: Data pattern, insights, itemsets, association rules

## Sentiment Analysis
### Problem Statement
A finales del mes de Junio, a raiz de la crisis sanitaria producto del COVID-19, se cuestionó que las clínicas privadas en Perú cobraban exorbitantes sumas por el tratamiento de pacientes infectados por el COVID-19 y que no tenían seguro privado. Ante esto el gobierno del Perú dio un ultimatum a las clínicas para llegar un acuerdo sobre las tarifas solidarias a cobrar por el tratamiento de pacientes con COVID-19. Ante esto se plantea conocer la percepción de la gente, su posición acerca de los anuncios dados por el gobierno sin necesidad de esperar una encuesta que tomaría más tiempo y recursos



Este proyecto tiene por finalidad medir la percepción de las personas en twitter sobre el acuerdo del gobierno con las clínicas privadas antes el COVID-19


![alt text][main-words]

[main-words]: https://github.com/rasecotineb/datascience/blob/master/sentiment-analysis/main-words-pos.JPG "Nube de palabras"


![alt text][roc-curve]

[roc-curve]: https://github.com/rasecotineb/datascience/blob/master/sentiment-analysis/roc-curve-sentyment-analysis.JPG "Curva ROC"

Visitar notebook de [sentiment analysis](https://github.com/rasecotineb/datascience/blob/master/sentiment-analysis/Twitter_Analisis_de_Sentimientos.ipynb)

>Tópicos: NLP, Bag of words, TFIDF, API Twitter, Naive Bayes
## 6. Exploratory Data Analysis
En análisis exploratorio de datos que se muestra a continuación se basa en el análisis descriptivo de la información de un dataset que permita el mayor entendimiento posible sobre la data mediante el uso de elementos gráficos como: *diagrama de barras, boxplot, heatmaps, entre otros*
>Tópicos: Plotting, Boxplot, Correlation
