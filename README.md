# Predicción del abandono de clientes bancarios — Beta Bank

## 1. Descripción del proyecto

Este proyecto desarrolla un modelo de *machine learning* para predecir qué clientes de Beta Bank podrían abandonar la institución.

El objetivo es identificar a los clientes con mayor probabilidad de cancelar sus servicios, de manera que el banco pueda diseñar estrategias de retención y reducir la pérdida de clientes.

## 2. Objetivo

Construir un modelo de clasificación binaria que prediga la variable `Exited`, que indica si un cliente abandonó el banco.

**Criterio principal de evaluación:** obtener un valor de F1 de al menos 0.59 y evaluar también el desempeño mediante el área bajo la curva ROC (AUC-ROC).

## 3. Proceso de trabajo

El proyecto comprende las siguientes etapas:

- Exploración y preparación de los datos.
- División de los datos en conjuntos de entrenamiento, validación y prueba.
- Entrenamiento y evaluación de modelos de clasificación.
- Análisis del desequilibrio entre las clases.
- Comparación de estrategias para mejorar la detección de clientes que abandonan el banco.
- Ajuste del umbral de clasificación utilizando el conjunto de validación.
- Evaluación final del modelo seleccionado con el conjunto de prueba.

## 4. Modelos y evaluación

Se compararon modelos de clasificación y estrategias para abordar el desequilibrio de clases. La selección consideró la métrica F1 y el AUC-ROC.

El umbral de clasificación se ajustó con el conjunto de validación. Posteriormente, el modelo seleccionado se evaluó con los datos de prueba para estimar su desempeño final.

## 5. Resultados finales

El modelo final obtuvo los siguientes resultados en el conjunto de prueba:

| Métrica | Resultado |
|---|---:|
| F1 | 0.630 |
| AUC-ROC | 0.865 |
| F1 mínimo requerido | 0.590 |

El modelo superó el valor mínimo de F1 establecido para el proyecto. El resultado de AUC-ROC refleja también una capacidad de discriminación entre clientes que abandonan el banco y aquellos que permanecen.

## 6. Tecnologías utilizadas

- Python
- pandas y NumPy
- scikit-learn
- Matplotlib y Seaborn
- Jupyter Notebook

## 7. Archivos del proyecto

- `beta_bank_trabajo.ipynb`: notebook con el análisis, el entrenamiento de modelos y la evaluación de resultados.
- `README.md`: descripción general del proyecto y sus resultados.

**Nota:** el archivo de datos `Churn.csv` no se incluye en este repositorio. Para reproducir el análisis, será necesario contar con el conjunto de datos original y ajustar su ruta de acceso en el notebook, si corresponde.

## 8. Conclusión

El proyecto demuestra cómo aplicar técnicas de aprendizaje automático para abordar un problema de clasificación relacionado con la retención de clientes bancarios. La comparación de modelos, el tratamiento del desequilibrio de clases y el ajuste del umbral permitieron obtener un modelo que cumple con el criterio mínimo de F1 establecido.

Este trabajo forma parte de mi formación práctica en ciencia de datos y refleja la aplicación de técnicas de análisis de datos y modelado predictivo a un problema de negocio del sector financiero.
