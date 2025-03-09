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

![Texto alternativo](C:\VSC\personal\imagenes\)

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

#### Parte 2: Cálculo y Análisis del Índice de Vegetación Quemada Normalizado (NBR)  
<p style="font-size: larger;">
A partir de imágenes satelitales post-incendio de Sentinel-2, se calculó el Índice de Vegetación Quemada Normalizado (NBR), lo que permitió evaluar la severidad de los incendios y la extensión de las áreas afectadas. El NBR se visualizó mediante una paleta de colores para facilitar la identificación de las zonas impactadas por el fuego.
</p>

<p style="font-size: larger;">
<strong>Conclusión</strong>:  
Esta práctica mostró cómo geemap y Google Earth Engine (GEE) pueden ser herramientas poderosas para realizar análisis geoespaciales avanzados. A través del uso de datasets del Earth Engine Data Catalog, los usuarios pueden obtener, procesar y visualizar datos de manera eficiente, lo que abre un abanico de posibilidades para la investigación y monitoreo de fenómenos naturales como la topografía del terreno y los efectos de los incendios.
</p>

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

#### Parte 2: Visualización del Límite Geográfico de Knox County  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Filtrar Knox County en Tennessee y visualizar sus límites con un borde rojo y sin relleno, en un mapa interactivo.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se cargó y filtró la colección de condados de EE.UU. para identificar el condado de <strong>Knox</strong>, y se visualizó en un mapa interactivo. Se agregó un texto para identificar al creador y personalizar la presentación.
</p>

#### Parte 3: Visualización de Imágenes de Landsat-9 para el condado de Knox  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Cargar imágenes Landsat-9, aplicar una máscara de nubes, seleccionar la imagen con menor cobertura nubosa y visualizarla en un mapa.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se filtraron las imágenes de Landsat-9 para <strong>Knox County</strong> entre junio y diciembre de 2023. Se aplicó un proceso de enmascarado de nubes, y se utilizó una combinación de bandas <strong>7-6-4</strong> para crear una visualización combinada en colores naturales con el objetivo de mostrar la cobertura terrestre.
</p>

#### Parte 4: Visualización de Imágenes de Sentinel-2 con Combinación de Bandas Infrarrojas  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Filtrar y procesar imágenes de Sentinel-2, crear un mosaico de las imágenes disponibles y visualizarlas utilizando la combinación de bandas <strong>Color Infrarrojo (5-4-3)</strong>.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se filtra el conjunto de imágenes de Sentinel-2 para obtener las imágenes más claras de <strong>Knox County</strong>, creando un mosaico de la combinación de bandas <strong>5-4-3</strong>. Esta combinación resalta la vegetación y la cobertura del suelo en colores infrarrojos.
</p>

#### Parte 5: Visualización de Imágenes de NAIP con Combinación de Bandas NIR, Rojo y Verde  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Utilice las imágenes de <strong>NAIP</strong> para generar una visualización con la combinación de bandas <strong>Color Infrarrojo (NIR, Rojo, Verde)</strong>.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se cargaron las imágenes de <strong>NAIP</strong> para <strong>Knox County</strong> y se creó un mosaico con las imágenes disponibles, visualizando la imagen resultante utilizando la combinación de bandas <strong>NIR, R, G</strong>, lo que permite visualizar la vegetación y la calidad de la cobertura terrestre.
</p>

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

#### Parte 3: Análisis y Visualización del Modelo Digital de Elevación (DEM) en la Cuenca Hidrográfica de Utah  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Generar un análisis del Modelo Digital de Elevación (DEM) para un área específica de Utah y visualizar los datos de elevación sobre las cuencas hidrográficas.
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se cargó el <strong>DEM (Modelo Digital de Elevación)</strong> de 10 metros de resolución proporcionado por <strong>USGS</strong> y se recortó a la cuenca hidrográfica de Utah previamente seleccionada. Los datos de elevación fueron visualizados con una paleta de colores que representa diferentes niveles de altitud, lo que permitió observar el relieve de la región y analizar la topografía de la zona.
</p>

#### Parte 4: Cambio en la Cobertura de Suelo entre 2001 y 2019 en Utah  
<p style="font-size: larger;">
<strong>Objetivo</strong>: Analizar los cambios en la cobertura del suelo en el estado de Utah entre los años 2001 y 2019 utilizando el conjunto de datos de <strong>NLCD</strong> (National Land Cover Database).
</p>

<p style="font-size: larger;">
<strong>Descripción</strong>:  
Se utilizaron las imágenes del <strong>NLCD</strong> de 2001 y 2019 para visualizar los cambios en el uso del suelo en Utah. Para facilitar la comparación, se empleó una visualización en panel dividido que muestra las imágenes de ambos años, permitiendo observar las diferencias en la cobertura de suelo. Además, se añadió una leyenda para identificar los tipos de cobertura de suelo y se usaron colores específicos para diferenciar las categorías.
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
