# Pokémon Legendary Classification

<img src="https://img.shields.io/badge/Python-3.11-blue?logo=python">
<img src="https://img.shields.io/badge/Scikit--learn-F7931E?logo=scikit-learn&logoColor=white">
<img src="https://img.shields.io/badge/Status-Completed-brightgreen">

Proyecto de **Machine Learning** para predecir si un Pokémon es legendario o no, usando aprendizaje supervisado con datos públicos.

## Descripción

Este proyecto analiza datos de Pokémon, realiza limpieza y análisis exploratorio de datos (EDA), y entrena modelos de machine learning para **clasificar Pokémon legendarios**.

Incluye:
- Limpieza de datos (eliminación de megas, formas alternas, etc.)
- Visualización de estadísticas y tipos
- Comparación de varios modelos de clasificación
- Evaluación e interpretación de resultados
- Validación con Pokémon nuevos

---

## EDA y Preprocesamiento

- Distribución de tipos, generaciones y stats de Pokémon
- Identificación de outliers y análisis de legendarios con stats altos
- Limpieza de datos para mantener solo las formas base
- Transformación de variables categóricas (One-Hot Encoding de tipos)
- Creación de features como “dual-type”


## Modelos

Se entrenaron y compararon los siguientes modelos:
- **Logistic Regression**
- **Gradient Boosting**
- **KNN**
- **XGBoost**
- *(Opcional: Random Forest, si lo incluiste)*

Se evaluaron con **accuracy**, **precision**, **recall** y **F1-score** para la clase legendario.

---

## Resultados

| Modelo                | Accuracy | F1 (Legendario) | Recall (Legendario) | Precision (Legendario) |
|-----------------------|----------|-----------------|---------------------|------------------------|
| Logistic Regression   | 0.979    | 0.842           | 1.00                | 0.727                  |
| Gradient Boosting     | 0.950    | 0.588           | 0.625               | 0.556                  |
| KNN                   | 0.964    | 0.615           | 0.500               | 0.800                  |
| XGBoost               | 0.971    | 0.750           | 0.750               | 0.750                  |

**Conclusión:**  
Logistic Regression fue el modelo más robusto para identificar legendarios (recall = 1.0), aunque con algunos falsos positivos.

---

## Ejemplos de Predicción

Pruebas con Pokémon legendarios y no legendarios de la 8va generación (no vistos por el modelo) mostraron que el modelo **clasifica correctamente ambos casos**, demostrando capacidad de generalización.

