# Clasificación de Marketing Bancario

Este proyecto implementa un modelo de aprendizaje supervisado para predecir el éxito de las campañas de marketing directo de una institución bancaria. El objetivo es determinar si un cliente contratará un depósito a plazo fijo basándose en sus atributos demográficos y comportamiento financiero previo.

## Contenido del Archivo

* **Bank Marketing.ipynb**: Notebook que contiene el análisis de datos, el preprocesamiento de variables categóricas y el entrenamiento del modelo de clasificación.

## Requerimientos de Software

Para la correcta ejecución de este notebook, se requiere la instalación de las siguientes librerías de Python. Las versiones listadas corresponden a las especificaciones técnicas del entorno de desarrollo:

* numpy (v1.26.x)
* pandas (v2.1.x)
* scikit-learn
* matplotlib
* seaborn (v0.13.x)
* ucimlrepo (v0.0.7)

## Entorno de Ejecución Recomendado

Se recomienda el uso de **Google Colab**. El entorno facilita la gestión de dependencias y permite la conexión directa con el repositorio de la UCI para la descarga automática del dataset mediante el ID 222.

---

## Persistencia del Modelo

El notebook incluye una sección de guardado del modelo entrenado mediante la librería `pickle`.

* **Archivo generado**: `finalized_model_bank_marketing.sav`
* **Propósito**: Permitir la reutilización del modelo en aplicaciones de predicción en tiempo real sin necesidad de reentrenamiento.

| Etapa | Descripción |
| :--- | :--- |
| Carga | Uso de ucimlrepo (id=222) para obtener features y targets. |
| Evaluación | Cálculo de métricas de precisión (Accuracy Score). |
| Visualización | Generación de Matrices de Confusión mediante ConfusionMatrixDisplay. |
