# Deteccion de basurales a cielo abierto

## Descripción

Los basurales a cielo abierto son aquellos donde los residuos se disponen de forma indiscriminada y con escasas medidas de protección ambiental. Esto es un problema en diferentes áreas, no sólo a nivel ecológico ambiental sino también a nivel sociedad, salud, y urbanización regulada.

Este proyecto tiene por objetivo la detección y seguimiento de los basurales a cielo abierto, aplicando técnicas basadas en machine learning (ML) para el procesamiento de imágenes satelitales. Esto permite mapear grandes áreas de manera rápida y con bajos recursos.

![](img_readme/A.png)![](img_readme/B.png)

El modelo está optimizado para las imágenes multiespectrales del satélite Sentinel-2. 

## Requerimientos

Se utilizan las herramientas **GDAL** y [Orfeo Toolbox](https://www.orfeo-toolbox.org/) en la primera etapa del pre-procesamiento de los datos. Luego, se emplean nuestros paquetes [satproc](https://github.com/dymaxionlabs/satproc) y [unetseg](https://github.com/dymaxionlabs/satproc) para la generación del dataset y modelo de ML respectivamente.

## Notebooks

Este repositorio contiene un conjunto de notebooks de Jupyter, que describen los pasos necesarios:

1. [Pre-procesamiento](notebooks/1_Preprocesamiento.ipynb): Se procesan las imágenes satelitales y la verdad de campo para generar el dataset de entrenamiento y de predicción del modelo.
2. [Entrenamiento](notebooks/2_Entrenamiento.ipynb): Entrenamiento y evaluación del modelo.
3. [Predicción](notebooks/3_Prediccion.ipynb): Predicción sobre la región de interés.
4. [Post Procesamiento](notebooks/4_Post-procesamiento.ipynb): Procesamiento de los resultados de la predicción.
