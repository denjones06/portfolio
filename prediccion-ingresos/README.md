# Predicción de Ingresos

## Objetivo
Desarrollar un modelo predictivo que estime el ingreso mensual de un cliente (en UYU) a partir de variables financieras y de comportamiento, minimizando el error relativo medio (MAPE).

## Descripción del problema
El conjunto de datos incluye información sobre saldos vigentes y vencidos, contingencias, calificaciones crediticias, número de instituciones financieras reportantes y variables demográficas.  
El objetivo es capturar relaciones complejas entre estas variables para predecir el ingreso mensual de forma precisa.

## Metodología
Se evaluaron múltiples enfoques de modelado, comenzando por modelos base y avanzando hacia técnicas más complejas.  
El proceso incluyó:

- Análisis exploratorio de datos.
- Imputación de valores faltantes (KNN Imputer e Iterative Imputer).
- Manejo de outliers mediante Z-score.
- Transformaciones y preparación de variables.
- Optimización de hiperparámetros mediante validación cruzada.
- Comparación de desempeño entre distintos modelos.

El modelo final seleccionado fue **XGBoost**, debido a su mejor desempeño en términos de MAPE y su capacidad para capturar relaciones no lineales.

## Evaluación
La métrica utilizada fue el **error relativo medio (MAPE)**.  
El modelo basado en XGBoost mostró un desempeño sólido en el conjunto de validación, con un MAPE cercano al **12%**, superando los benchmarks definidos.

## Resultados
El modelo entrenado se utilizó para generar predicciones sobre el conjunto de prueba.  
Los resultados finales fueron exportados a un archivo **CSV** con las predicciones de ingreso mensual.

## Conclusión
La combinación de un preprocesamiento robusto, imputación iterativa, manejo de outliers y optimización de hiperparámetros permitió construir un modelo preciso y estable para la predicción de ingresos.

### Nota
Por motivos de confidencialidad, los datasets utilizados para el entrenamiento y la evaluación no se incluyen en este repositorio.  
El código permite reproducir el pipeline completo utilizando datos locales.
