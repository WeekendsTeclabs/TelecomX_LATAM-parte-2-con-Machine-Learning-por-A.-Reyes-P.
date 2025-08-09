# TelecomX_LATAM-parte-2-con-Machine-Learning-por-A.-Reyes-P.
Este proyecto tiene como objetivo analizar y predecir la cancelación (churn) de clientes en un servicio, utilizando técnicas de análisis de datos y modelos de machine learning. Se abordan pasos desde la exploración de datos, análisis estadístico, hasta el entrenamiento y evaluación de modelos predictivos.

# Proyecto Análisis de Churn de Clientes

## Descripción

Este proyecto tiene como objetivo analizar y predecir la cancelación (churn) de clientes en un servicio, utilizando técnicas de análisis de datos y modelos de machine learning. Se abordan pasos desde la exploración de datos, análisis estadístico, hasta el entrenamiento y evaluación de modelos predictivos.

---

## Contenido del Proyecto

- Análisis exploratorio de la variable objetivo y variables predictoras.
- Preparación de datos: tratamiento de variables categóricas y numéricas.
- Entrenamiento de modelos de clasificación: Regresión Logística y Random Forest.
- Implementación adicional de Regresión Lineal para análisis exploratorio.
- Evaluación de modelos con métricas clásicas (classification report, AUC) y regresión (RMSE, R²).
- Interpretación de resultados y análisis de importancia de variables.
- Desarrollo de un plan estratégico para reducción de churn basado en insights.

---

## Estructura de Archivos

- `notebook.ipynb` (o script `.py`): Código completo con procesamiento, modelado y visualización.
- `data/`: Carpeta con datos crudos y procesados.
- `README.md`: Documento con explicación del proyecto y pasos realizados.

---

## Paso a Paso del Proyecto

### 1. Análisis Exploratorio

- Cálculo de la tasa global de churn y análisis por categorías relevantes (`gender`, `contract type`, `internet service`).
- Visualización con gráficos de barras y boxplots para entender distribución y diferencias.

### 2. Preparación de Datos

- Conversión de variables categóricas a variables dummy para modelado.
- Conversión y limpieza de variables numéricas (`TotalCharges`).
- División de datos en entrenamiento y prueba (75%-25%) con estratificación.

### 3. Escalado

- Aplicación de `StandardScaler` para normalizar variables numéricas y mejorar convergencia de modelos.

### 4. Entrenamiento de Modelos

- Regresión Logística con ajuste de hiperparámetros básicos.
- Random Forest con 100 árboles para capturar relaciones no lineales.
- Regresión Lineal como análisis exploratorio adicional para evaluar relaciones lineales directas.

### 5. Evaluación de Modelos

- Para clasificación:
  - Reporte de clasificación (precisión, recall, F1-score).
  - Matriz de confusión visual.
  - Curva ROC y cálculo de AUC.
- Para regresión:
  - RMSE y R² para evaluar ajuste del modelo lineal.
  - Gráficos de predicción vs valores reales.

### 6. Interpretación

- Análisis de métricas para determinar el mejor modelo.
- Identificación de variables con mayor importancia según Random Forest.
- Visualización y entendimiento del impacto de variables sobre churn.

### 7. Conclusión Estratégica

- Resumen de factores clave que influyen en la cancelación.
- Propuesta de plan de acción para retención y reducción de churn.

---

## Requisitos y Librerías

```bash
pip install pandas numpy scikit-learn matplotlib seaborn statsmodels
