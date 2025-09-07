#  Maintenance Categorization of Oil-Immersed Transformers Based on Machine Learning

Este repositorio contiene la implementación del método propuesto en el artículo:

**“Maintenance Categorization of Oil-Immersed Transformers Based on Machine Learning”**  
*Juan David García Correa – Armando Jaime Ustariz Farfán*  

El código automatiza la **clasificación del estado de transformadores de potencia sumergidos en aceite** a partir de parámetros fisicoquímicos del fluido dieléctrico, integrando técnicas de **Machine Learning (K-Means + XGBoost)** para apoyar estrategias de mantenimiento **CBM (Condition-Based Maintenance)**.

---

##  Metodología

El pipeline implementado consta de tres fases principales:

1. **Segmentación (K-Means)**  
   - Agrupamiento no supervisado de transformadores según variables fisicoquímicas.  
   - Visualización 2D y 3D de clústeres.  
   - Cálculo de métricas de cohesión (Silhouette Score).  

2. **Clasificación supervisada (XGBoost)**  
   - Entrenamiento de un modelo con etiquetas generadas en la segmentación.  
   - Evaluación mediante matriz de confusión, exactitud y recall por clase.  

3. **Predicción de mantenimiento (CBM)**  
   - Traducción de los clústeres en acciones de mantenimiento correctivo, preventivo o rutinario.  
   - Priorización de equipos en función del riesgo operativo.  

---

##  Variables fisicoquímicas

El análisis se basa en seis parámetros del aceite dieléctrico:

- Tensión interfacial  
- Número ácido  
- Rigidez dieléctrica  
- Contenido de humedad  
- Furanos (2-FAL)  
- Índice de calidad  

Base de datos: **180 transformadores en operación en el sistema eléctrico colombiano**.

---

##  Resultados destacados

- **Silhouette Score (K=3):** 0.62  
- **Exactitud XGBoost:** ~89 %  
- **Recall por clúster:** superior al 85 % en todas las clases.  

El método propuesto logra **clasificación automática confiable** y genera un plan de mantenimiento **priorizado por criticidad**.  

---



