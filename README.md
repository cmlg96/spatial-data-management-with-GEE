# 🌍 **Prácticas con Google Earth Engine en Python** 🐍

¡Hola! 👋 Este repositorio contiene 7 prácticas personalizadas que realicé mientras aprendía a utilizar **Google Earth Engine** (GEE) en **Python**. Estos ejercicios forman parte del curso "**Gestión de datos espaciales con Google Earth Engine**", impartido por el profesor **Qiusheng Wu** del **Instituto Universitario de las Naciones Unidas para el Agua, el Medio Ambiente y la Salud**. 🎓

Mi objetivo es compartir estas prácticas para ayudar a quienes quieran empezar a programar con GEE desde Python. Si bien están inspiradas en el curso, los códigos son de creación propia, por lo que cada práctica es completamente personalizable y adaptable a diferentes necesidades. 🚀

---

## 📚 **Prácticas del curso**

### **Práctica 1: Crear un mapa interactivo utilizando Leafmap en Python** 🐍

**Objetivo**: Crear un mapa interactivo utilizando Leafmap en Python, agregando elementos visuales y geoespaciales.

**Elementos añadidos**:
- Mapa interactivo centrado en una ubicación específica.
- Mapa base en estilo "CartoDB.DarkMatter".
- Texto personalizado en el mapa para mostrar la autoridad o etiquetas.
- Logo con imagen personalizada en la esquina inferior derecha.
- Datos GeoJSON: Carga de un archivo GeoJSON de Europa, con un estilo de perfilado azul y relleno transparente.

**Resultado**: Generación de un mapa interactivo con los elementos mencionados.

---

### **Práctica 2: Creación de un Mapa Interactivo con geemap, Personalización de Texto, Logo y Datos GeoJSON** 📊

**Objetivo**: Crear un mapa interactivo utilizando geemap en Python, agregando varios elementos visuales como texto, imágenes y datos geoespaciales con estilo.

**Elementos añadidos**:
- Mapa interactivo centrado en una ubicación específica.
- Mapa base en estilo "CartoDB.DarkMatter".
- Texto personalizado en el mapa para mostrar la autoridad o etiquetas.
- Logo con imagen personalizada en la esquina inferior derecha.
- Datos GeoJSON: Carga de un archivo GeoJSON de Europa, con un estilo de perfilado azul y relleno transparente.

**Resultado**: Generación de un mapa interactivo con los elementos anteriores, incluyendo el estilo de los datos geoespaciales.

---

### **Práctica 3: Análisis y Visualización de Datasets del Earth Engine Data Catalog con geemap** 🔥

**Objetivo**: Familiarizarse con el uso de geemap y Google Earth Engine (GEE) para trabajar con datasets del Earth Engine Data Catalog, específicamente en la visualización de datos geoespaciales y el análisis de fenómenos como la elevación del terreno y el impacto de incendios mediante el Índice de Vegetación Quemada Normalizado (NBR) en imágenes satelitales post-incendio.

**Parte 1**: **Visualización de un Modelo Digital de Superficie (DSM)**  
Se seleccionó un Modelo Digital de Elevación (DEM) de los disponibles en Earth Engine para generar un DSM de una región de interés. Este modelo se visualizó utilizando una paleta de colores que representaba las diferentes elevaciones del terreno, ayudando a obtener una representación detallada del relieve geográfico de la zona seleccionada.

**Parte 2**: **Cálculo y Análisis del Índice de Vegetación Quemada Normalizado (NBR)**  
A partir de imágenes satelitales post-incendio de Sentinel-2, se calculó el Índice de Vegetación Quemada Normalizado (NBR), lo que permitió evaluar la severidad de los incendios y la extensión de las áreas afectadas. El NBR se visualizó mediante una paleta de colores para facilitar la identificación de las zonas impactadas por el fuego.

**Conclusión**:  
Esta práctica mostró cómo geemap y Google Earth Engine (GEE) pueden ser herramientas poderosas para realizar análisis geoespaciales avanzados. A través del uso de datasets del Earth Engine Data Catalog, los usuarios pueden obtener, procesar y visualizar datos de manera eficiente, lo que abre un abanico de posibilidades para la investigación y monitoreo de fenómenos naturales como la topografía del terreno y los efectos de los incendios.

---

### **Práctica 4: Análisis y Visualización de Imágenes Satélites para el Estudio de Condiciones Territoriales con geemap y Earth Engine** ⚙️

**Objetivos**:
- Aprender a trabajar con geemap y Google Earth Engine para acceder a diferentes tipos de datos geoespaciales.
- Realizar análisis y visualizaciones de imágenes satelitales como las de Landsat-9, Sentinel-2 y NAIP para el estudio de áreas específicas, como **Knox County**, Tennessee.
- Filtrar, procesar y representar datos geográficos (como límites administrativos) y aplicar análisis de cobertura terrestre con imágenes satelitales.

**Parte 1**: **Filtrado de Datos y Creación de DataFrame**  
**Objetivo**: Filtrar una colección de datos geoespaciales para encontrar registros específicos (en este caso, "Knox"), convertirlos en un DataFrame y agregar una columna numerada.

**Descripción**:  
Se cargaron los límites de condados de EE.UU. desde Earth Engine, filtrando por el nombre de "Knox" y convirtiendo el conjunto filtrado en un DataFrame. Este proceso facilita la visualización y manipulación de los datos tabulares.

---

**Parte 2**: **Visualización del Límite Geográfico de Knox County**  
**Objetivo**: Filtrar Knox County en Tennessee y visualizar sus límites con un borde rojo y sin relleno, en un mapa interactivo.

**Descripción**:  
Se cargó y filtró la colección de condados de EE.UU. para identificar el condado de **Knox**, y se visualizó en un mapa interactivo. Se agregó un texto para identificar al creador y personalizar la presentación.

---

**Parte 3**: **Visualización de Imágenes de Landsat-9 para el condado de Knox**  
**Objetivo**: Cargar imágenes Landsat-9, aplicar una máscara de nubes, seleccionar la imagen con menor cobertura nubosa y visualizarla en un mapa.

**Descripción**:  
Se filtraron las imágenes de Landsat-9 para **Knox County** entre junio y diciembre de 2023. Se aplicó un proceso de enmascarado de nubes, y se utilizó una combinación de bandas **7-6-4** para crear una visualización combinada en colores naturales con el objetivo de mostrar la cobertura terrestre.

---

**Parte 4**: **Visualización de Imágenes de Sentinel-2 con Combinación de Bandas Infrarrojas**  
**Objetivo**: Filtrar y procesar imágenes de Sentinel-2, crear un mosaico de las imágenes disponibles y visualizarlas utilizando la combinación de bandas **Color Infrarrojo (5-4-3)**.

**Descripción**:  
Se filtra el conjunto de imágenes de Sentinel-2 para obtener las imágenes más claras de **Knox County**, creando un mosaico de la combinación de bandas **5-4-3**. Esta combinación resalta la vegetación y la cobertura del suelo en colores infrarrojos.

---

**Parte 5**: **Visualización de Imágenes de NAIP con Combinación de Bandas NIR, Rojo y Verde**  
**Objetivo**: Utilice las imágenes de **NAIP** para generar una visualización con la combinación de bandas **Color Infrarrojo (NIR, Rojo, Verde)**.

**Descripción**:  
Se cargaron las imágenes de **NAIP** para **Knox County** y se creó un mosaico con las imágenes disponibles, visualizando la imagen resultante utilizando la combinación de bandas **NIR, R, G**, lo que permite visualizar la vegetación y la calidad de la cobertura terrestre.

---

¡Eso es todo! Espero que sea útil y visualmente atractivo. Puedes copiar este código directamente en tu archivo Markdown para tener la estructura completa. ¡Espero que te sirva! 🚀

---



## 🎯 Objetivo del repositorio

Estas prácticas son **totalmente personalizadas** y las he subido aquí porque creo que pueden ser muy útiles para quienes están empezando con Google Earth Engine en Python. 🛠️ Mi idea es que sirvan como guía y punto de partida para explorar las increíbles capacidades de GEE. 🌟

---

## 🌟 ¿Por qué estas prácticas?

- **Aprendizaje práctico**: Cada práctica está diseñada para aplicar conceptos teóricos en situaciones reales. 🧠
- **Personalización**: Los ejercicios están adaptados a mis necesidades, pero son lo suficientemente flexibles para que otros los utilicen. 🛠️
- **Comunidad**: Quiero contribuir a la comunidad de GEE y Python compartiendo lo que he aprendido. 🤝

---

## 🚀 ¿Cómo usar este repositorio?

1. Clona el repositorio en tu máquina local.
2. Instala las dependencias necesarias (como `geemap` y `earthengine-api`).
3. Explora las prácticas en orden o salta directamente a la que más te interese.
4. ¡Experimenta y modifica los códigos para adaptarlos a tus necesidades! 💻

---

## 🙏 Agradecimientos

Un enorme agradecimiento al profesor **Qiusheng Wu** por su curso y por compartir su conocimiento con la comunidad. Sin su guía, estas prácticas no habrían sido posibles. 🙌

---

¡Espero que estas prácticas te sean útiles y que disfrutes explorando el mundo de Google Earth Engine en Python! 🌍🐍

¡Gracias por visitar este repositorio! 😊
