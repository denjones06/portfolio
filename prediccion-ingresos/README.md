# Predicción de Ingresos

## Objetivo
Desarrollar un modelo predictivo que estime el ingreso mensual de un cliente (en UYU) a partir de variables financieras y de comportamiento, minimizando el error relativo medio (MAPE).

## Descripción del problema
El conjunto de datos incluye información sobre saldos vigentes y vencidos, contingencias, calificaciones crediticias, número de instituciones financieras reportantes y variables demográficas. El objetivo es capturar relaciones complejas entre estas variables para predecir el ingreso mensual.

## Metodología
Se evaluaron múltiples enfoques de modelado, comenzando por modelos base y avanzando hacia técnicas más complejas.  
El proceso incluyó:
- Análisis exploratorio de datos.
- Imputación de valores faltantes (KNN Imputer e Iterative Imputer).
- Manejo de outliers mediante Z-score.
- Transformaciones de variables.
- Optimización de hiperparámetros mediante validación cruzada.
- Comparación de desempeño entre distintos modelos.

El modelo final seleccionado fue XGBoost, debido a su mejor desempeño en términos de MAPE y su capacidad para capturar relaciones no lineales.

## Evaluación
La métrica utilizada fue el error relativo medio (MAPE).  
El modelo final obtuvo un MAPE aproximado de **12.29%** en el conjunto de validación.

## Resultados
El modelo entrenado se utilizó para generar predicciones sobre el conjunto de prueba, y los resultados fueron exportados a un archivo CSV con las predicciones finales.

## Conclusión
La combinación de un preprocesamiento robusto, imputación iterativa, manejo de outliers y optimización de hiperparámetros permitió construir un modelo preciso y estable para la predicción de ingresos.
