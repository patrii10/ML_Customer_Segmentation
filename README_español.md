#  ML_Customer_Clustering  

Este proyecto tiene como objetivo analizar un conjunto de datos de clientes mayoristas, para identificar patrones y segmentar a los clientes en grupos. 

---

## **Descripción del proyecto**
Utilizando información sobre las compras en categorías como alimentos frescos, lácteos, productos de limpieza... hemos realizado un análisis exploratorio empleando Machine Learning para entender mejor el comportamiento de los clientes y agruparlos en diferentes segmentos según sus hábitos de compra.

Una vez hecho esto, haremos uso de los grupos para crear estrategias de marketing especificas a cada grupo. 

---

## **Objetivo principal**
El objetivo es identificar las características que principales que agrupan a los clientes, para crear grupos que permitan hacer recomendaciones de marketing personalizadas.

> ¿Cuáles son los principales patrones de compra entre los clientes y cómo podemos segmentarlos?

---

## **Contenido del análisis**

1. **Introducción**
   - Descripción del problema: El objetivo es segmentar clientes en diferentes grupos basados en sus patrones de compra.

2. **Hipótesis inicial**
   - Se plantea que los clientes se pueden segmentar en base a  sus compras en diferentes categorías como alimentos frescos, lácteos, productos de limpieza...
   - Se busca encontrar relaciones entre las diferentes categorías de productos comprados y características de los clientes.

3. **Exploración de datos**
   - Análisis de variables clave como:
     - Compras en **Fresh**, **Milk**, **Grocery**, **Frozen**, **Detergents_Paper**, **Delicassen**.
     - Relación de estas variables con la **Región** y el **Canal** de ventas.
   - Análisis de la distribución de los datos, identificación de outliers y transformaciones realizadas para mejorar la calidad de los datos.
   
4. **Resultados clave**
   - Identificación de patrones de compra y distribución de clientes.
   - Normalización y transformación de los datos (logaritmos y escalado) para preparar el dataset para el clustering.
   - Creación de segmentos de clientes usando técnicas de clustering.

5. **Conclusiones**
   - Reflexiones finales sobre los grupos de clientes identificados.
   - Posibles estrategias de marketing o ventas basadas en los grupos segmentados.

---

## Dataset  
- **Nombre**: Wholesale Customers Data  
- **Fuente**: [Kaggle](https://www.kaggle.com/datasets/binovi/wholesale-customers-data-set/data)  
- **Descripción**: Contiene información sobre clientes de un mayorista y sus patrones de compra en distintas categorías de productos.  
- **Tamaño**: 440 filas, 8 columnas.
---

## **Herramientas utilizadas**
- **Python**: Para el análisis de datos.
   - **Bibliotecas**: Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn.
- **Jupyter Notebook**: Entorno de trabajo para ejecutar el análisis.
- **Clustering**: KMeans para la segmentación de clientes.
- **Transformaciones**: Normalización y transformación logarítmica de los datos.

---

## Estructura del repositorio  
📁 `src/data_sample/` → Muestra del dataset  
📁 `src/img/` → Gráficos y visualizaciones  
📁 `src/notebooks/` → Notebooks de prueba  
📁 `src/results_notebook/` → Notebook final con el modelo  
📁 `src/models/` → Modelos guardados  
📁 `src/utils/` → Funciones auxiliares  

## Metodología  
1. **Exploración de los datos (EDA)**  
2. **Preprocesamiento y normalización**  
3. **Aplicación de técnicas de clustering**  
4. **Evaluación de los resultados**  
5. **Conclusiones y mejoras futuras**  
6. **Exportación de modelos**

---

### **Resultados principales**

- Se aplicaron distintos algoritmos de clustering: `KMeans`, `DBSCAN` y `Agglomerative`.
- La reducción de dimensionalidad mediante `PCA` permitió mantener el **93% de la varianza** en solo 4 componentes.
- Se evaluaron los modelos con la métrica **Silhouette Score** para determinar la cohesión de los clusters:

| Algoritmo             | Silhouette Score |
|-----------------------|------------------|
| **KMeans (sin PCA)**  | 0.64             |
| **KMeans (con PCA)**  | 0.69             |
| **DBSCAN**            | 0.79             |
| **Agglomerative**     | 0.78             |

- Finalmente se eligió **KMeans con PCA (k=2)** como modelo óptimo por su equilibrio entre:
  - Simplicidad de implementación  
  - Buena separación visual  
  - Robustez ante nuevos datos  
  - Interpretabilidad para perfiles de clientes

---


