# Estrategia de Clasificación para la Evaluación del Mantenimiento de Transformadores Sumergidos en Aceite Basada en Machine Learning

En este repositorio se presenta una **estrategia metodológica** que permite la clasificación y priorización del mantenimiento de transformadores de potencia en servicio, a partir de los **parámetros fisicoquímicos del aceite dieléctrico**.  
La estrategia propuesta integra técnicas de **aprendizaje automático** para apoyar el esquema de **Condition-Based Maintenance (CBM)** en sistemas eléctricos de potencia.

La metodología está compuesta por tres fases principales:  
1. **Segmentación con K-Means** → agrupamiento no supervisado de transformadores en categorías de condición.  
2. **Clasificación con XGBoost** → entrenamiento de un modelo supervisado con etiquetas generadas en la segmentación.  
3. **Predicción de mantenimiento (CBM)** → traducción de las clases técnicas en planes de acción (correctivo, preventivo o rutinario).  

Cada fase se describe en el código y en las tablas/figuras generadas, garantizando **transparencia y reproducibilidad** en el proceso.  

---

## ¿Qué puedes encontrar en este repositorio?

En este repositorio encontrarás el código fuente y los datos utilizados para implementar la metodología planteada en el artículo.  

### Estructura del repositorio

- **`Maintenance_Categorization_of_Oil_Immersed_Transformers_Based_on_Machine_Learning.ipynb`**  
  Notebook de Jupyter/Colab con la implementación paso a paso de la metodología, incluyendo código, resultados intermedios y explicaciones.

- **`maintenance_categorization_of_oil_immersed_transformers_based_on_machine_learning.py`**  
  Script en Python generado a partir del notebook, listo para ejecutarse directamente en cualquier entorno local.
  

---

##  Tecnologías utilizadas

- Python 3.x  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost  

---





