# 🌍 Prácticas con Google Earth Engine en Python 🐍

<p style="font-size: larger;">
¡Hola! 👋 Este repositorio contiene 7 prácticas personalizadas que realicé mientras aprendía a utilizar <strong>Google Earth Engine (GEE)</strong> en <strong>Python</strong>. Estos ejercicios forman parte del curso <strong>"Gestión de datos espaciales con Google Earth Engine"</strong>, impartido por el profesor <strong>Qiusheng Wu</strong> del <strong>Instituto Universitario de las Naciones Unidas para el Agua, el Medio Ambiente y la Salud</strong>. 🎓
</p>

<p style="font-size: larger;">
Mi objetivo es compartir estas prácticas para ayudar a quienes quieran empezar a programar con GEE desde Python. Si bien están inspiradas en el curso, los códigos son de creación propia, por lo que cada práctica es completamente personalizable y adaptable a diferentes necesidades. 🚀
</p>

---

## 📚 Prácticas del curso

### Práctica 1: Crear un mapa interactivo utilizando Leafmap en Python 🐍

<p style="font-size: larger;">
<strong>Objetivo</strong>: Crear un mapa interactivo utilizando Leafmap en Python, agregando elementos visuales y geoespaciales.
</p>

<p style="font-size: larger;">
<strong>Elementos añadidos</strong>:
</p>

- Mapa interactivo centrado en una ubicación específica.
- Mapa base en estilo "CartoDB.DarkMatter".
- Texto personalizado en el mapa para mostrar la autoridad o etiquetas.
- Logo con imagen personalizada en la esquina inferior derecha.
- Datos GeoJSON: Carga de un archivo GeoJSON de Europa, con un estilo de perfilado azul y relleno transparente.

<p style="font-size: larger;">
<strong>Resultado</strong>: Generación de un mapa interactivo con los elementos mencionados.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_01.JPG)
---

### Práctica 2: Creación de un Mapa Interactivo con geemap, Personalización de Texto, Logo y Datos GeoJSON 📊

<p style="font-size: larger;">
<strong>Objetivo</strong>: Crear un mapa interactivo utilizando geemap en Python, agregando varios elementos visuales como texto, imágenes y datos geoespaciales con estilo.
</p>

<p style="font-size: larger;">
<strong>Elementos añadidos</strong>:
</p>

- Mapa interactivo centrado en una ubicación específica.
- Mapa base en estilo "CartoDB.DarkMatter".
- Texto personalizado en el mapa para mostrar la autoridad o etiquetas.
- Logo con imagen personalizada en la esquina inferior derecha.
- Datos GeoJSON: Carga de un archivo GeoJSON de Europa, con un estilo de perfilado azul y relleno transparente.

<p style="font-size: larger;">
<strong>Resultado</strong>: Generación de un mapa interactivo con los elementos anteriores, incluyendo el estilo de los datos geoespaciales.
</p>

---

### Práctica 3: Análisis y Visualización de Datasets del Earth Engine Data Catalog con geemap 🔥

<p style="font-size: larger;">
<strong>Objetivo</strong>: Familiarizarse con el uso de geemap y Google Earth Engine (GEE) para trabajar con datasets del Earth Engine Data Catalog, específicamente en la visualización de datos geoespaciales y el análisis de fenómenos como la elevación del terreno y el impacto de incendios mediante el Índice de Vegetación Quemada Normalizado (NBR) en imágenes satelitales post-incendio.
</p>

#### Parte 1: Visualización de un Modelo Digital de Superficie (DSM)  
<p style="font-size: larger;">
Se seleccionó un Modelo Digital de Elevación (DEM) de los disponibles en Earth Engine para generar un DSM de una región de interés. Este modelo se visualizó utilizando una paleta de colores que representaba las diferentes elevaciones del terreno, ayudando a obtener una representación detallada del relieve geográfico de la zona seleccionada.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_03_A.JPG)

#### Parte 2: Cálculo y Análisis del Índice de Vegetación Quemada Normalizado (NBR)  
<p style="font-size: larger;">
A partir de imágenes satelitales post-incendio de Sentinel-2, se calculó el Índice de Vegetación Quemada Normalizado (NBR), lo que permitió evaluar la severidad de los incendios y la extensión de las áreas afectadas. El NBR se visualizó mediante una paleta de colores para facilitar la identificación de las zonas impactadas por el fuego.
</p>

<p style="font-size: larger;">
<strong>Conclusión</strong>:  
Esta práctica mostró cómo geemap y Google Earth Engine (GEE) pueden ser herramientas poderosas para realizar análisis geoespaciales avanzados. A través del uso de datasets del Earth Engine Data Catalog, los usuarios pueden obtener, procesar y visualizar datos de manera eficiente, lo que abre un abanico de posibilidades para la investigación y monitoreo de fenómenos naturales como la topografía del terreno y los efectos de los incendios.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_03_B.JPG)

---

### Práctica 4: Análisis y Visualización de Imágenes Satélites para el Estudio de Condiciones Territoriales con geemap y Earth Engine ⚙️

<p style="font-size: larger;">
<strong>Objetivo</strong>:
</p>

- Aprender a trabajar con geemap y Google Earth Engine para acceder a diferentes tipos de datos geoespaciales.
- Realizar análisis y visualizaciones de imágenes satelitales como las de Landsat-9, Sentinel-2 y NAIP para el estudio de áreas específicas, como <strong>Knox County</strong>, Tennessee.
- Filtrar, procesar y representar datos geográficos (como límites administrativos) y aplicar análisis de cobertura terrestre con imágenes satelitales.

#### Parte 1: Filtrado de Datos y Creación de DataFrame  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Filtrar una colección de datos geoespaciales para encontrar registros específicos (en este caso, "Knox"), convertirlos en un DataFrame y agregar una columna numerada.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se cargaron los límites de condados de EE.UU. desde Earth Engine, filtrando por el nombre de "Knox" y convirtiendo el conjunto filtrado en un DataFrame. Este proceso facilita la visualización y manipulación de los datos tabulares.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_04_A.JPG)

#### Parte 2: Visualización del Límite Geográfico de Knox County  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Filtrar Knox County en Tennessee y visualizar sus límites con un borde rojo y sin relleno, en un mapa interactivo.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se cargó y filtró la colección de condados de EE.UU. para identificar el condado de <strong>Knox</strong>, y se visualizó en un mapa interactivo. Se agregó un texto para identificar al creador y personalizar la presentación.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_04_B.JPG)

#### Parte 3: Visualización de Imágenes de Landsat-9 para el condado de Knox  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Cargar imágenes Landsat-9, aplicar una máscara de nubes, seleccionar la imagen con menor cobertura nubosa y visualizarla en un mapa.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se filtraron las imágenes de Landsat-9 para <strong>Knox County</strong> entre junio y diciembre de 2023. Se aplicó un proceso de enmascarado de nubes, y se utilizó una combinación de bandas <strong>7-6-4</strong> para crear una visualización combinada en colores naturales con el objetivo de mostrar la cobertura terrestre.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_04_C.JPG)

#### Parte 4: Visualización de Imágenes de Sentinel-2 con Combinación de Bandas Infrarrojas  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Filtrar y procesar imágenes de Sentinel-2, crear un mosaico de las imágenes disponibles y visualizarlas utilizando la combinación de bandas <strong>Color Infrarrojo (5-4-3)</strong>.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se filtra el conjunto de imágenes de Sentinel-2 para obtener las imágenes más claras de <strong>Knox County</strong>, creando un mosaico de la combinación de bandas <strong>5-4-3</strong>. Esta combinación resalta la vegetación y la cobertura del suelo en colores infrarrojos.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_04_D.JPG)

#### Parte 5: Visualización de Imágenes de NAIP con Combinación de Bandas NIR, Rojo y Verde  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Utilice las imágenes de <strong>NAIP</strong> para generar una visualización con la combinación de bandas <strong>Color Infrarrojo (NIR, Rojo, Verde)</strong>.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se cargaron las imágenes de <strong>NAIP</strong> para <strong>Knox County</strong> y se creó un mosaico con las imágenes disponibles, visualizando la imagen resultante utilizando la combinación de bandas <strong>NIR, R, G</strong>, lo que permite visualizar la vegetación y la calidad de la cobertura terrestre.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_04_E.JPG)

---

### Práctica 5: Manipulación de Cuencas Hidrográficas (USGS WBD), Modelos Digitales de Elevación (DEM), Análisis de Cobertura del Suelo (NLCD) y Visualización de Datos de OpenStreetMap con Geemap

<p style="font-size: larger;">
<strong>Objetivo</strong>:
</p>

- Explorar conjuntos de datos geoespaciales, como cuencas hidrográficas, modelos digitales de elevación (DEM), y cambios en la cobertura del suelo.
- Localización de restaurantes en Salt Lake City utilizando datos de <strong>OpenStreetMap</strong>.
- Uso de herramientas de visualización y procesamiento de datos para entender los procesos naturales y humanos.

#### Parte 1: Límites de Cuencas Hidrográficas en EE.UU.  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Visualizar los límites de las cuencas hidrográficas en los Estados Unidos utilizando el <strong>USGS Watershed Boundary Dataset (WBD)</strong>.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
En esta parte se cargaron los límites de las cuencas hidrográficas de los EE.UU. a partir del conjunto de datos <strong>USGS Watershed Boundary Dataset</strong>. Las cuencas hidrográficas, o áreas de drenaje, son regiones donde el agua fluye hacia un mismo punto de salida, como un río o lago. Se aplicó un estilo para representar estas cuencas en un mapa interactivo, con un borde azul y sin relleno, permitiendo observar las zonas que definen el drenaje a nivel nacional.
</p>

#### Parte 2: Intersección de Cuencas Hidrográficas con el Estado de Utah  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Mostrar cómo las cuencas hidrográficas se intersectan con una zona específica, en este caso el estado de Utah, para entender cómo las áreas de drenaje interactúan con las fronteras políticas.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
En esta parte, se cargaron los límites de los condados de <strong>Utah</strong> y las fronteras del estado, utilizando los conjuntos de datos de <strong>TIGER</strong>. Luego, se filtraron las cuencas hidrográficas que intersectan con el estado y se visualizó este conjunto de datos en un mapa. Se añadió un estilo diferenciando las cuencas hidrográficas y las fronteras estatales con colores específicos para facilitar su identificación visual.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_05_2_.JPG)

#### Parte 3: Análisis y Visualización del Modelo Digital de Elevación (DEM) en la Cuenca Hidrográfica de Utah  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Generar un análisis del Modelo Digital de Elevación (DEM) para un área específica de Utah y visualizar los datos de elevación sobre las cuencas hidrográficas.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se cargó el <strong>DEM (Modelo Digital de Elevación)</strong> de 10 metros de resolución proporcionado por <strong>USGS</strong> y se recortó a la cuenca hidrográfica de Utah previamente seleccionada. Los datos de elevación fueron visualizados con una paleta de colores que representa diferentes niveles de altitud, lo que permitió observar el relieve de la región y analizar la topografía de la zona.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_05_3_.JPG)

#### Parte 4: Cambio en la Cobertura de Suelo entre 2001 y 2019 en Utah  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Analizar los cambios en la cobertura del suelo en el estado de Utah entre los años 2001 y 2019 utilizando el conjunto de datos de <strong>NLCD</strong> (National Land Cover Database).
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se utilizaron las imágenes del <strong>NLCD</strong> de 2001 y 2019 para visualizar los cambios en el uso del suelo en Utah. Para facilitar la comparación, se empleó una visualización en panel dividido que muestra las imágenes de ambos años, permitiendo observar las diferencias en la cobertura de suelo. Además, se añadió una leyenda para identificar los tipos de cobertura de suelo y se usaron colores específicos para diferenciar las categorías.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_05_4_.JPG)

---
#### Parte 5: Localización de Restaurantes en Salt Lake City usando OSM y Geemap

<p style="font-size: larger;">
<strong>Objetivo</strong>: Utilizar las herramientas `osmnx` y `geemap` para extraer y visualizar los restaurantes de Salt Lake City a partir de datos de OpenStreetMap (OSM). El objetivo es demostrar cómo geolocalizar puntos de interés dentro de una área específica utilizando datos geoespaciales y presentarlos en un mapa interactivo.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Esta práctica se enfoca en la obtención de datos geoespaciales sobre restaurantes en Salt Lake City mediante la librería 'osmnx', que permite acceder fácilmente a la base de datos de OpenStreetMap. En primer lugar, se geocodifica la ciudad utilizando 'ox.geocode_to_gdf' para obtener las geometrías de Salt Lake City en formato GeoDataFrame. Luego, los datos del GeoDataFrame se convierten a un formato compatible con Google Earth Engine (EE) para su visualización en un mapa interactivo con `geemap`.

Posteriormente, se filtran los datos de OSM para obtener únicamente los restaurantes dentro de los límites de Salt Lake City, utilizando la etiqueta 'amenity=restaurant'. Los datos obtenidos se procesan para garantizar que las geometrías sean puntos, utilizando la función `handle_geometry` para convertir cualquier geometría que no sea un punto (como polígonos) en su respectivo punto central.

Finalmente, los restaurantes se visualizan en un mapa interactivo centrado en Salt Lake City, donde se añaden como puntos de color rojo. Este ejercicio demuestra cómo integrar datos geoespaciales de diferentes fuentes, como OSM y Google Earth Engine, para realizar análisis espaciales y crear visualizaciones interactivas en Python.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_05_5_.JPG)

---
### Práctica 6: Visualización y Análisis de Datos Geoespaciales con Google Earth Engine 🌍

<p style="font-size: larger;">
<strong>Objetivo</strong>: Usar Google Earth Engine (GEE) junto con la biblioteca geemap para cargar, procesar y visualizar distintos conjuntos de datos geoespaciales en un cuaderno de Jupyter. Esta práctica incluye el análisis de datos climáticos de NOAA, imágenes satelitales de Landsat y Sentinel-2, y análisis de datos agrícolas con el conjunto de datos de USDA NASS.
</p>

---

### Parte 1: Visualización de Datos Climáticos de NOAA 📊

<p style="font-size: larger;">
<strong>Objetivo</strong>: Cargar los datos de temperatura a 2 metros del modelo de pronóstico GFS de NOAA y visualizar las variaciones globales de temperatura en un mapa interactivo.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: En esta parte, se extrae la capa de temperatura a 2 metros del conjunto de datos NOAA GFS, utilizando las imágenes de pronóstico de este sistema global de modelado. Se emplean parámetros de visualización como una paleta de colores y valores mínimos y máximos para resaltar las zonas de diferente temperatura en el mapa. La adición de un control de color y una barra de color proporciona una referencia visual precisa, facilitando la interpretación de los datos climáticos globales en tiempo real.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_06_1.JPG)

---

### Parte 2: Análisis de Imágenes de Landsat 7 🛰️

<p style="font-size: larger;">
<strong>Objetivo</strong>: Cargar y visualizar una imagen compuesta de Landsat 7 entre 1999 y 2003 utilizando diferentes combinaciones de bandas para el análisis de características geográficas.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: En esta parte, se utiliza una imagen compuesta de Landsat 7 (1999-2003) para evaluar diferentes características de la superficie terrestre a través de distintas combinaciones de bandas. Se emplean configuraciones específicas de visualización, como color natural, infrarrojo cercano y color falso para analizar áreas de vegetación, geología y humedad del suelo. Las imágenes se visualizan en un formato de mapa dividido para comparar los efectos de las diferentes combinaciones de bandas sobre la misma área geográfica, permitiendo una interpretación espacial detallada.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_06_2.JPG)

---

### Parte 3: Análisis Temporal con USDA NASS Cropland Data Layers 🌾

<p style="font-size: larger;">
<strong>Objetivo</strong>: Visualizar los cambios en el uso del suelo agrícola desde 2010 hasta 2022 usando las capas de datos del USDA NASS y analizar la variabilidad temporal mediante un inspector de series temporales.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: Aquí se trabaja con el conjunto de datos de la capa de uso agrícola del USDA NASS, que proporciona información anual sobre el uso de tierras en los EE. UU. desde 2010 hasta 2022. Se utiliza el inspector de series temporales para evaluar cómo ha cambiado el uso del suelo en una región específica, visualizando las diferentes clases de uso agrícola a lo largo del tiempo. Esta sección permite observar las variaciones en las zonas de cultivo y las transiciones entre diferentes tipos de uso del suelo mediante una comparación de capas de diferentes años.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_06_3.JPG)

---

### Parte 4: Análisis de Imágenes de Sentinel-2 en Knoxville, TN 🌍

<p style="font-size: larger;">
<strong>Objetivo</strong>: Filtrar y visualizar imágenes de Sentinel-2 para la ciudad de Knoxville, TN, con menos del 10% de cobertura nubosa para análisis temporal utilizando bandas NIR, Roja y Verde.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: En este paso se filtran imágenes de Sentinel-2 usando criterios espaciales y temporales para obtener solo aquellas con menos del 10% de nubosidad, enfocándose en el área de Knoxville, TN. Las imágenes seleccionadas se visualizan utilizando bandas del infrarrojo cercano (NIR), rojo y verde, lo que permite realizar análisis sobre la vegetación, monitorización del terreno y salud de las áreas verdes. La incorporación de un control deslizante temporal permite explorar cómo ha cambiado la ciudad durante un período de tiempo determinado, lo que facilita el análisis de tendencias a lo largo de los años.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_06_4.JPG)

---

### Parte 5: Comparación de Cobertura del Suelo con ESA World Cover y Landsat 🌱

<p style="font-size: larger;">
<strong>Objetivo</strong>: Comparar las imágenes de cobertura del suelo de ESA World Cover con las de Landsat, utilizando un mapa dividido para observar diferencias en el uso del suelo y la vegetación.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: En esta sección se comparan dos conjuntos de datos: ESA World Cover y Landsat, para analizar la cobertura del suelo en EE. UU. Se recortan ambos conjuntos de imágenes a las fronteras de los estados de EE. UU. para una visualización más precisa. Se utilizan dos mapas divididos para mostrar simultáneamente ambas coberturas y permitir la comparación directa de las diferencias en la clasificación del suelo. La adición de una leyenda para ESA World Cover facilita la interpretación de las clases de cobertura del suelo. Además, se agregan los límites geográficos de los estados de EE. UU. para mejorar el contexto geoespacial.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_06_5.JPG)

---

### Práctica 7: Análisis de Imágenes Satelitales para Claiborne County, Tennessee 📡

<p style="font-size: larger;">
<strong>Objetivo</strong>: Realizar un análisis geoespacial completo utilizando Google Earth Engine y geemap para visualizar, descargar y analizar imágenes satelitales de diferentes fuentes, como Landsat 7, Landsat 8, Sentinel-2 y NAIP, para el condado de Claiborne, Tennessee.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: 
Esta práctica permite realizar un análisis de imágenes satelitales del condado de Claiborne utilizando distintas fuentes de datos. Se carga y visualiza una imagen de Landsat 7, sobre la cual se aplican parámetros de visualización y se sobrepone una cuadrícula para facilitar la interpretación. Además, se utiliza Landsat 8 para un análisis temporal de las imágenes de 2017 a 2023, aplicando una máscara para las nubes. También se calculan y visualizan índices como el NDVI a partir de imágenes de Sentinel-2, específicamente entre los meses de junio a agosto de cada año, y se trabaja con imágenes de NAIP en color falso para observar cambios en el uso de la tierra y vegetación de 2010 a 2023. Finalmente, se descarga tanto la información geoespacial como las imágenes procesadas para su posterior análisis y uso en SIG.
</p>

<p style="font-size: larger;">
<strong>Resultado</strong>: Generación de un conjunto de imágenes satelitales procesadas, análisis geoespacial interactivo y descargas de imágenes de alta calidad de diferentes fuentes para el análisis temporal y espacial en el condado de Claiborne.
</p>

---

### Parte 1: Carga y Visualización de Imágenes de Landsat 7 con Cuadrícula Fishnet 🛰️

<p style="font-size: larger;">
<strong>Objetivo</strong>: Cargar una imagen de Landsat 7, aplicar parámetros de visualización y superponer una cuadrícula tipo fishnet para analizar la región geográfica seleccionada.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: 
Esta sección carga una imagen de Landsat 7 del periodo 1999-2003 y la visualiza utilizando un esquema de color específico (bandas B4, B3 y B2). Se añade una cuadrícula tipo fishnet sobre la imagen, con una resolución ajustable, que sirve como referencia para analizar las imágenes de satélite y hacer análisis espaciales detallados.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_07_1.JPG)

---

### Parte 2: Análisis Temporal con Imágenes de Landsat 8 para Claiborne County 🗓️

<p style="font-size: larger;">
<strong>Objetivo</strong>: Filtrar y analizar imágenes de Landsat 8 para el condado de Claiborne entre 2017 y 2023, aplicando una máscara de nubes y visualizando el cambio temporal.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: 
En esta parte, se filtran las imágenes de Landsat 8 por el área de Claiborne County entre los años 2017 y 2023, aplicando una máscara para nubes. Se utiliza el método de mediana para generar una imagen compuesta que reduce las nubes y proporciona una visión más clara de los cambios en la superficie terrestre a lo largo del tiempo.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_07_2.JPG)

---

### Parte 3: Cálculo y Visualización del NDVI con Imágenes de Sentinel-2 🌱

<p style="font-size: larger;">
<strong>Objetivo</strong>: Calcular el Índice de Vegetación de Diferencia Normalizada (NDVI) utilizando imágenes de Sentinel-2 durante los meses de verano entre 2018 y 2023.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: 
Se utilizan imágenes de Sentinel-2 para calcular el NDVI en el condado de Claiborne durante los meses de junio a agosto de los años 2018 a 2023. El NDVI se utiliza para analizar la salud y la cobertura vegetal, donde los valores cercanos a 1 indican vegetación densa y los valores cercanos a -1 indican áreas sin vegetación.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_07_3.JPG)

---

### Parte 4: Visualización de Imágenes NAIP en Color Falso (NIR-R-G) de 2010 a 2023 🌍

<p style="font-size: larger;">
<strong>Objetivo</strong>: Visualizar las imágenes anuales de NAIP en el condado de Claiborne entre 2010 y 2023 utilizando una combinación de bandas en falso color (NIR-R-G).
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: 
En esta sección se procesan imágenes de NAIP utilizando las bandas de infrarrojo cercano (NIR), rojo (R) y verde (G) para generar imágenes en falso color que ayudan a identificar cambios en la vegetación y el uso del suelo. Se visualizan imágenes anuales entre 2010 y 2023 para observar las tendencias a largo plazo en el área.
</p>

![alt text](https://github.com/cmlg96/practice/blob/main/lab_07_4.JPG)

---

### Parte 5: Descarga de Límites Geográficos de Claiborne County como Shapefile y GeoJSON 🗺️

<p style="font-size: larger;">
<strong>Objetivo</strong>: Descargar los límites geográficos del condado de Claiborne en formato Shapefile y GeoJSON para su uso en sistemas de información geográfica (SIG).
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>: 
Se descarga el límite geográfico del condado de Claiborne a partir de la base de datos de condados de EE. UU. y se guarda en formatos Shapefile y GeoJSON, que son ampliamente utilizados en SIG para realizar análisis espaciales detallados.
</p>

---
## 🎯 Objetivo del repositorio

<p style="font-size: larger;">
Estas prácticas son <strong>totalmente personalizadas</strong> y las he subido aquí porque creo que pueden ser muy útiles para quienes están empezando con Google Earth Engine en Python. 🛠️ Mi idea es que sirvan como guía y punto de partida para explorar las increíbles capacidades de GEE. 🌟
</p>

---

## 🌟 ¿Por qué estas prácticas?

<p style="font-size: larger;">
</p>

- <strong>Aprendizaje práctico</strong>: Cada práctica está diseñada para aplicar conceptos teóricos en situaciones reales. 🧠
- <strong>Personalización</strong>: Los ejercicios están adaptados a mis necesidades, pero son lo suficientemente flexibles para que otros los utilicen. 🛠️
- <strong>Comunidad</strong>: Quiero contribuir a la comunidad de GEE y Python compartiendo lo que he aprendido. 🤝

---

## 🚀 ¿Cómo usar este repositorio?

<p style="font-size: larger;">
</p>

1. Clona el repositorio en tu máquina local.
2. Instala las dependencias necesarias (como <code>geemap</code> y <code>earthengine-api</code>).
3. Explora las prácticas en orden o salta directamente a la que más te interese.
4. ¡Experimenta y modifica los códigos para adaptarlos a tus necesidades! 💻

---

## 🙏 Agradecimientos

<p style="font-size: larger;">
Un enorme agradecimiento al profesor <strong>Qiusheng Wu</strong> por su curso y por compartir su conocimiento con la comunidad. Sin su guía, estas prácticas no habrían sido posibles. 🙌
</p>

---

<p style="font-size: larger;">
¡Espero que estas prácticas te sean útiles y que disfrutes explorando el mundo de Google Earth Engine en Python! 🌍🐍
</p>

<p style="font-size: larger;">
¡Gracias por visitar este repositorio! 😊
</p>
