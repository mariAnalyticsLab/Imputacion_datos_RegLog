# Imputacion_datos_RegLog

## ✔️ Descripción del problema
En muchos conjuntos de datos reales existen valores faltantes, los cuales pueden afectar el análisis estadístico y el desempeño de modelos de aprendizaje automático. En este proyecto, los valores faltantes están representados por el valor 0, lo cual requiere una estrategia de imputación para completar la información de forma coherente.
Este script aborda el problema de completar datos faltantes en un dataset tabular utilizando un enfoque de aprendizaje automático supervisado, específicamente el algoritmo Gaussian Naive Bayes.

## ✔️ Funcionamiento
- El script recibe un archivo CSV con datos numéricos.
- Se define una estructura fija de 76 filas y 40 colum nas, rellenando con ceros en caso de valores faltantes.
- El valor 0 se considera como dato faltante.
Para cada columna:
- Se seleccionan los casos completos (valores distintos de cero).
- Se entrena un modelo Gaussian Naive Bayes usando el resto de las columnas como variables predictoras.
- Se predicen los valores faltantes de manera individual.
- Los valores imputados se almacenan en un nuevo DataFrame.
- El resultado final se guarda en un nuevo archivo CSV.

## ✔️ Herramientas y tecnologías utilizadas
Lenguaje
- Python 3
Librerías
- pandas
- numpy
- scikit-learn
- GaussianNB

## ✔️ Datos
- Este repositorio no incluye datos reales sensibles.
- El archivo de entrada (datos1.csv) contiene datos numéricos utilizados con fines académicos y de experimentación.
- El archivo de salida (datoscompletos1.csv) corresponde al dataset con los valores imputados.

## ✔️ Resultados y aprendizajes obtenidos
- Imputación automatizada de valores faltantes mediante modelos probabilísticos.
- Uso de aprendizaje supervisado para completar información incompleta.
- Manejo de datasets con dimensiones fijas.
- Aplicación práctica de Naive Bayes en un problema distinto a la clasificación tradicional.
- Fortalecimiento del flujo de trabajo con pandas y scikit-learn.

## ✔️ Limitaciones
- El valor 0 se asume como dato faltante, lo cual puede no ser válido para todos los conjuntos de datos.
- La calidad de la imputación depende de la cantidad y distribución de los datos completos.
- El proceso puede ser computacionalmente costoso en datasets más grandes.
- No se realiza validación estadística de las predicciones imputadas.

## ✔️ Disclaimer
Este proyecto tiene fines educativos y de aprendizaje, y no pretende sustituir métodos estadísticos avanzados de imputación ni ser utilizado directamente en entornos productivos sin validación adicional.
