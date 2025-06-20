# Predicción de Ocupación en Airbnb

## Descripción del Proyecto

Este proyecto implementa un modelo de Machine Learning para predecir la **ocupación alta o baja** de propiedades listadas en Airbnb en Buenos Aires. El objetivo es ayudar a los anfitriones a optimizar estrategias de precios y maximizar la ocupación y los ingresos.

---

## Datos

- Dataset obtenido mediante scraping de Airbnb en marzo de 2024.
- Incluye características de las propiedades como ubicación, tipo, capacidad, precios, número de reseñas y calificaciones.
- La variable objetivo es la ocupación binaria, donde:
  - `1` = alta ocupación (más del 80%)
  - `0` = baja ocupación

---

## Metodología

- Limpieza y preparación de datos.
- Ingeniería de características (feature engineering) para variables numéricas y categóricas.
- Balanceo de clases mediante oversampling para evitar sesgos.
- Modelo principal: Random Forest Classifier.
- Validación cruzada y evaluación con métricas como F1-score, matriz de confusión y curva ROC-AUC.
- Análisis de importancia de variables para interpretación del modelo.

---

## Resultados

- El modelo alcanzó un F1-score promedio de aproximadamente 0.93 en validación cruzada.
- La curva ROC-AUC mostró un desempeño excelente (~0.99).
- Variables más importantes incluyen: `minimum_nights`, `longitude`, `maximum_nights` y `price`.

---

## Uso

El proyecto está desarrollado en Python con Jupyter Notebook (`.ipynb`), que contiene todo el flujo: desde la carga de datos, procesamiento, entrenamiento, evaluación y visualización.

---

Elaborado por:

- Abril Noguera
- José R. Castro