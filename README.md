# Deteccion de basurales a cielo abierto


Los basurales a cielo abierto son aquellos donde los residuos se disponen de forma indiscriminada y con escasas medidas de protección ambiental. Esto es un problema en diferentes áreas, no solo a nivel ecológico ambiental sino también a nivel sociedad, salud, y urbanización regulada.
Este proyecto tiene por objetivo la detección y seguimiento de los basurales a cielo abierto, aplicando técnicas basadas en machine learning (ML) para el procesamiento de imágenes satelitales. Esto permite mapear grandes áreas de manera rápida y con bajos recursos.


El modelo está optimizado para las imágenes del satélite Sentinel-2. Y se utilizan las herramientas de **GDAL** y **ORFEO** en la primera etapa del pre-procesamiento de los datos. Y se emplean las librerías del **pysatproc** y **unetseg** de python para la generación del dataset y modelo de ML respectivamente.

## Notebooks
* **Pre-procesamiento:** Se procesan las imágenes satelitales y la verdad de campo para generar el dataset de entrenamiento y de predicción del modelo.
* **Entrenamiento:** Entrenamiento y evaluación del modelo.
* **Predicción:** Predicción sobre la región de interés.
* **Post Procesamiento:** procesamiento de los resultados de la predicción.
