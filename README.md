# IA_Jupyter

Regresion lineal: Es un modelo estadístico que busca encontrar la relación lineal entre una variable independiente (X) y una dependiente (Y).
Se representa con la fórmula: Y = aX + b
Donde:
a es la pendiente (cuánto cambia Y si X cambia)
b es la ordenada al origen (valor de Y cuando X = 0)
✅ Se usa para predecir valores o detectar tendencias.

Árbol de Decisión: es un algoritmo de aprendizaje automático supervisado que se utiliza para clasificación o regresión. Funciona como un diagrama tipo árbol, donde cada nodo representa una decisión basada en los valores de las variables.
✅ ¿Cuándo usar un árbol de decisión?
Necesitas un modelo interpretable y fácil de explicar
Trabajas con datos estructurados (columnas tipo Excel o base de datos)
Tienes tanto variables categóricas como numéricas
Quieres resolver problemas de clasificación o regresión
No quieres preocuparte por la normalización o escalado de datos
Tienes un dataset pequeño o mediano
Necesitas saber por qué se llegó a cierta predicción

Algoritmos de clustering no supervisado: DBSCAN y K-Means
🎯 PROPÓSITO DE DBSCAN
Objetivo principal: Detectar áreas densas de puntos y agruparlos, sin necesidad de definir cuántos clusters hay, y separando automáticamente los outliers (ruido).
✅ Ideal para:
Datos con formas irregulares (no circulares)
Datos con ruido o outliers
Agrupaciones con diferente densidad
Cuando no sabes cuántos grupos hay

DBSCAN: Es un algoritmo de agrupamiento (clustering) que forma clusters en base a la densidad de puntos en el espacio.
Agrupa puntos que están cerca unos de otros (eps) y forman regiones densas (min_samples)
Detecta y separa automáticamente los outliers (ruido)
✅ Útil cuando los clusters no tienen forma circular y hay ruido en los datos.

🎯 PROPÓSITO DE K-MEANS
Objetivo principal:Agrupar datos en K grupos definidos por centroides, minimizando la distancia entre los puntos y su centro.
✅ Ideal para:
Datos con clusters esféricos o circulares
Agrupaciones con densidades similares
Cuando ya sabes cuántos grupos necesitas (k)
Agrupaciones rápidas y eficientes

K-Means: Es un algoritmo de agrupamiento (clustering) no supervisado que forma K clusters basados en la distancia a centroides (puntos centrales).
✅¿Cuándo usar K-Means?
Cuando sabes cuántos clusters quieres (k)
Cuando los datos tienen grupos bien separados y de forma circular
Cuando necesitas un algoritmo rápido y simple
Cuando no te preocupan los outliers
Cuando haces segmentación inicial o exploratoria

Clusters:  Son grupos de datos similares entre sí, creados por un algoritmo de clustering.
Cada cluster agrupa puntos que comparten alguna característica común o están cerca entre sí en el espacio.
✅ En DBSCAN, los clusters se forman por densidad.

Scatter: (Scatter plot o Diagrama de dispersión)
Es un tipo de gráfico que muestra la relación entre dos variables numéricas.
Cada punto en el gráfico representa un par de valores (X, Y) de una observación.
✅ Sirve para visualizar patrones, agrupaciones o tendencias.

Clase: En POO, una clase es una plantilla o modelo que define cómo debe ser un objeto: qué atributos tiene y qué puede hacer (métodos).
✅ La clase es como una receta o plano.

Instancia: Es un objeto específico creado a partir de una clase.
Cuando usas una clase y creas un “ejemplar” real con ella, eso es una instancia.
✅ Puedes tener muchas instancias de una misma clase, con distintos valores.

