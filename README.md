# FC25_K-means
<h1>Proyecto de Aprendizaje No Supervisado: Clasificación de Jugadores FC25</h1>

<p>Este proyecto se enfoca en el aprendizaje no supervisado con el objetivo de clasificar a los jugadores del popular videojuego FC25 (FIFA) en cuatro grupos o <strong>clusters</strong>. Para lograr esto, se implementará el algoritmo k-means en cuatro variantes distintas, utilizando tres métricas diferentes para medir la similitud entre los jugadores: distancia Euclideana, distancia Mahalanobis y distancia L1. La visualización de los resultados se llevará a cabo mediante Análisis de Componentes Principales (<strong>PCA</strong>).</p>

<h2>Descripción del Conjunto de Datos</h2>
<p>El conjunto de datos consta de información detallada sobre los jugadores, que incluye diversas características relevantes para la clasificación (se proporcionará una breve descripción de las variables en dos líneas).</p>

<h2>Exploración de Datos (EDA)</h2>
<p>Se realizará un análisis exploratorio de los datos (EDA) que incluirá:</p>

<ul>
        <li><strong>Selección de Variables:</strong> Identificación de las variables más significativas que se utilizarán en el análisis.</li>
        <li><strong>Escalado de Variables:</strong> Aplicación de técnicas de escalado para asegurar que las variables estén en la misma escala, lo que es crucial para la correcta aplicación del algoritmo k-means.</li>
</ul>

<p>Además, se llevará a cabo la imputación de datos faltantes y se codificará la variable correspondiente al pie preferido de los jugadores en una variable binaria, lo que facilitará su inclusión en el análisis.</p>

<h2>Implementación del Algoritmo k-means</h2>
<h3>1. Implementación Usando Librerías</h3>
<p>Se utilizarán librerías estándar de Python, como Scikit-learn, para aplicar el algoritmo k-means de manera eficiente y efectiva.</p>

<h3>2. Implementación Manual</h3>
    <p>Se desarrollará una implementación manual del algoritmo k-means, permitiendo una comprensión más profunda del funcionamiento del mismo. Esta implementación utilizará tres tipos diferentes de distancias para calcular la similitud: Euclideana, Mahalanobis y L1.</p>

<h2>Descripción del Algoritmo k-means</h2>
    <p>El algoritmo k-means es un método de clasificación no supervisada que tiene las siguientes características clave:</p>
<ul>
        <li><strong>Clasificación No Supervisada:</strong> No requiere etiquetas previas para clasificar los datos.</li>
        <li><strong>Limitaciones Estructurales:</strong> No es adecuado para estructuras de datos no convexas.</li>
        <li><strong>Sensibilidad a la Inicialización:</strong> La selección inicial de los centroides puede afectar significativamente los resultados.</li>
        <li><strong>Escalado de Datos:</strong> Es esencial que los datos estén adecuadamente escalados para garantizar un rendimiento óptimo del algoritmo.</li>
</ul>

<h2>Visualización y Reducción de Dimensionalidad</h2>
<p>Para facilitar la interpretación de los resultados, se aplicará PCA (Análisis de Componentes Principales) como técnica de reducción de dimensionalidad. Se seleccionarán tres componentes principales que preservan el 80% de la varianza de los datos. Esta transformación permitirá visualizar la clusterización en espacios bidimensionales (2D) y tridimensionales (3D), y los centroides de los clusters se representarán en este nuevo espacio para facilitar su análisis.</p>

