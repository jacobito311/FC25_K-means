# Proyecto EDA y K-means

## Primera parte: EDA
1. **Importación de librerías y carga de datos:**  
   El primer paso fue importar las librerías necesarias para el manejo y visualización de los datos. Utilizamos librerías populares como `numpy` para operaciones de álgebra lineal, `pandas` para la manipulación de dataframes, y `matplotlib` y `seaborn` para la generación de gráficos.

2. **Resumen estadístico y exploración inicial:**  
   Posteriormente, generamos un resumen estadístico de los datos para obtener una vista general de las principales características numéricas, como el promedio, desviación estándar, valores mínimos y máximos, entre otros. También revisamos la estructura del dataset, verificando el número de filas, columnas, tipos de datos y valores nulos. Esto nos permitió identificar rápidamente cualquier anomalía o valores que debieran ser tratados más adelante.

3. **Análisis de las ligas y nacionalidades:**  
   Realizamos un análisis de las 10 ligas con mayor cantidad de jugadores, visualizando los resultados mediante un gráfico de barras. Del mismo modo, analizamos la distribución de jugadores por nacionalidad y el valor promedio de la calificación general (OVR) por país, lo cual nos ayudó a entender mejor la representación global en el dataset.

4. **Distribución del OVR:**  
   Un aspecto clave del análisis fue la distribución del OVR (Overall Rating), una métrica fundamental en el dataset. Para esto, construimos un histograma que nos permitió observar cómo se distribuyen las calificaciones entre los jugadores. Adicionalmente, agregamos una curva de densidad que nos dio una mejor idea sobre la concentración de los valores.

5. **Análisis por posición:**  
   Exploramos las posiciones de los jugadores y su relación con el OVR. Mediante un diagrama de caja (boxplot), visualizamos cómo varían las calificaciones en función de la posición de los jugadores, lo cual reveló información valiosa sobre la distribución de habilidades entre diferentes roles en el campo.

6. **Matriz de correlación:**  
   Para identificar posibles relaciones entre atributos, generamos una matriz de correlación que nos mostró cómo variables como la velocidad (PAC), tiro (SHO), defensa (DEF), entre otras, se correlacionan entre sí y con el OVR. Esta matriz fue representada gráficamente mediante un mapa de calor que facilitó la interpretación visual de las correlaciones más significativas.

7. **Mejores jugadores y equipos:**  
   Finalmente, identificamos los jugadores con las mejores calificaciones dentro de cada liga, así como los equipos con los OVR medios más altos. Visualizamos los 30 equipos más destacados en un gráfico de barras, lo que nos permitió comprender mejor cómo se distribuyen los mejores jugadores entre los clubes.

## Segunda parte: Implementación del Algoritmo y Visualización de Resultados
En el proyecto, implementamos el algoritmo K-means con diferentes métricas de distancia para agrupar datos de interés. Cada uno de los integrantes del equipo trabajó con una métrica diferente: la distancia Euclidiana, la distancia de Manhattan, y la distancia de Mahalanobis.

Tras cargar los datos, procedimos a realizar una limpieza y preparación. Esto incluyó la imputación de valores faltantes, principalmente en las columnas relacionadas con los atributos de los porteros, donde los valores faltantes se reemplazaron por ceros.

Luego de esta fase inicial, aplicamos transformaciones adicionales sobre los datos. Esto incluyó la codificación de variables categóricas, como el pie preferido y la nacionalidad, mediante la técnica de codificación numérica. A continuación, utilizamos un imputador para reemplazar cualquier valor faltante restante con la mediana de cada columna.

El siguiente paso fue aplicar el método del codo para determinar el número óptimo de clusters (k) en cada una de las implementaciones. Graficamos el WCSS (Within-Cluster Sum of Squares) para diferentes valores de k y elegimos un valor adecuado basado en la visualización de la gráfica.

Una vez determinado el número de clusters, procedimos con la implementación del algoritmo K-means en cada una de las versiones (tipos de distancias).

Adicionalmente, implementamos una visualización de los resultados utilizando la técnica de Análisis de Componentes Principales (PCA), la cual nos permitió reducir las dimensiones de los datos y graficar los clusters en 2 y 3 dimensiones. De esta manera, logramos observar de manera más clara cómo se agruparon los datos y la distribución de los centroides en el espacio reducido.

Finalmente, los 3 miembros del equipo comparamos los resultados obtenidos con las diferentes distancias para evaluar cómo la elección de la métrica afectaba la calidad del clustering y la separación entre los grupos.
