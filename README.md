# Repositorio de Proyectos: Machine Learning y Análisis de Datos

Este repositorio contiene una colección de implementaciones técnicas que abarcan diversas ramas del aprendizaje automático, desde el aprendizaje supervisado (Clasificación y Regresión) hasta el aprendizaje no supervisado (Clustering) y técnicas de preprocesamiento avanzado (PCA).

## Contenido del Repositorio

1. **Bank Marketing.ipynb**: Modelo de clasificación binaria para predecir si un cliente se suscribirá a un depósito a plazo fijo. Utiliza el dataset de marketing bancario de la UCI para analizar comportamientos basados en campañas de telemarketing.

2. **customers_cluster.ipynb**: Implementación de segmentación de clientes mayoristas mediante K-Means. Agrupa a los usuarios según sus patrones de gasto anuales para identificar perfiles comerciales específicos.

3. **power_consumption.ipynb**: Análisis y predicción de series temporales aplicado al consumo eléctrico doméstico. Utiliza redes neuronales para estimar la demanda energética futura basándose en dependencias temporales.

4. **spambase_pca.ipynb**: Sistema de detección de correo no deseado que utiliza Análisis de Componentes Principales (PCA) para la reducción de dimensionalidad, optimizando el entrenamiento de una red neuronal de clasificación.

## Requerimientos de Software

Para la ejecución de cualquiera de los notebooks, se deben instalar las siguientes dependencias. Las versiones listadas garantizan la compatibilidad con los métodos de serialización utilizados:

* numpy (v1.26.x)
* pandas (v2.1.x)
* scikit-learn
* matplotlib
* seaborn (v0.13.x)
* ucimlrepo (v0.0.7)

## Entorno de Ejecución Recomendado

Se recomienda el uso de **Google Colab** para ejecutar estos archivos. El entorno proporciona las librerías necesarias preinstaladas y facilita la conexión con el `ucimlrepo` para la descarga automática de los datasets.

---

## Persistencia de Modelos

Todos los notebooks incluyen una fase de exportación mediante la librería `pickle`. Este proceso genera archivos con extensión `.sav` que permiten cargar los modelos entrenados en otros entornos sin necesidad de repetir el proceso de ajuste.

* **Ejemplo de carga**: `modelo = pickle.load(open('nombre_archivo.sav', 'rb'))`

| Proyecto | Objetivo Técnico | Dataset |
| :--- | :--- | :--- |
| Bank Marketing | Clasificación | UCI Bank Marketing |
| Customers Cluster | Clustering | Wholesale Customers |
| Power Consumption | Regresión (Series Temporales) | Household Power Consumption |
| Spambase PCA | Clasificación + PCA | Spambase |
