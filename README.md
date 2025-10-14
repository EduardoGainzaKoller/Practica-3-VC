# README - Práctica 3: Visión por Computador

## Autor: Eduardo Gainza Koller

## Introducción

Este documento acompaña al cuaderno de Jupyter **`VC_Practica3_EGK.ipynb`**, desarrollado como parte de la asignatura de Visión por Computador.

El presente trabajo tiene como objetivo la implementación de técnicas fundamentales de procesamiento digital de imágenes y visión artificial para resolver dos problemas clave: 
la detección de objetos circulares (monedas) y la clasificación y localización de microplásticos en imágenes complejas. Para ello, se ha empleado la librería 
**OpenCV** junto con **NumPy** y **Matplotlib**.

***

## Desarrollo de las Tareas

El cuaderno aborda dos tareas principales que demuestran los conocimientos antes mencionados:

### 1. Detección de Monedas

Esta sección se enfoca en el uso de técnicas de **detección de formas circulares** para identificar y contar automáticamente las monedas presentes en una imagen.

* **Metodología:** La implementación utiliza métodos estándar de OpenCV, como la binarización de la imagen, la detección de contornos y
* la **Transformada de Hough para Círculos**, para localizar los centros y radios de las monedas.
* **Resultado:** La imagen final muestra las monedas detectadas, marcadas con círculos o contornos, y proporciona el recuento total de objetos identificados.

<img width="236" height="466" alt="image" src="https://github.com/user-attachments/assets/832e9ba6-c73d-4002-9d8d-57b0bf5169bf" />

***

### 2. Clasificador de Microplásticos

El objetivo es aplicar técnicas de **detección y clasificación de objetos** para identificar y etiquetar microplásticos (MPs) en una imagen de prueba.

* **Metodología:** Se parte de un *dataset* (`df_test`) que contiene las coordenadas de las **cajas delimitadoras (`bounding boxes`)** para cada microplástico. El código procesa
* estas coordenadas y una etiqueta de predicción (`Prediction`) para visualizar los resultados.
* **Visualización de Resultados:** El cuaderno genera una imagen donde se superponen los *bounding boxes* a los microplásticos detectados. Cada caja se
* etiqueta indicando tanto la **etiqueta real (`R:`)** como la **etiqueta predicha (`P:`)**. Se emplean distintos colores para visualizar la clase predicha y
* compararla con la etiqueta verdadera.
* A continuación se muestran los resultados obtenidos:

<img width="728" height="735" alt="image" src="https://github.com/user-attachments/assets/2382f76a-3d1a-42c1-965b-69bbd2c48599" />
<img width="569" height="756" alt="image" src="https://github.com/user-attachments/assets/66d1af7c-fd04-400c-a368-85ad9281e74f" />

