# Clustering
Es una técnica de aprendizaje no supervisado que busca agrupar datos similares en subconjuntos llamados clusters o grupos,  
sin necesidad de etiquetas previas.  

**¿Cómo funciona?**
- El algoritmo analiza las características de los datos (variables)
- Calcula una métrica de similitud (como la distancia Euclídea)
- Agrupa en clusters los puntos que están más cerca entre sí  

El **objetivo** es que:
- Los elementos dentro de un mismo cluster sean muy parecidos
- Los elementos entre diferentes clusters sean muy distintos

## KMeans
K-Means es un algoritmo de clustering que agrupa instancias en K grupos (clusters) minimizando la distancia entre los puntos y el centroide del grupo al que pertenecen.  
- Asume que los clusters son esféricos y bien separados
- Requiere definir K (número de clusters) manualmente
- Se basa en la distancia Euclídea

✅ **¿Cuándo usar K-Means?**
- Los datos están bien distribuidos y separables
- Tienes una noción aproximada del número de grupos
- Buscas un algoritmo rápido y eficiente

## DBSCAN
Agrupa puntos densamente conectados y detecta automáticamente outliers.  
No requiere definir el número de clusters  
Agrupa puntos si hay una densidad suficiente  
Tiene dos parámetros importantes: eps (radio) y min_samples (mínimos puntos vecinos)  

✅ **¿Cuándo usar DBSCAN?**
- Hay clusters de forma irregular
- Quieres detectar ruido o valores atípicos
- No sabes cuántos grupos existen

## Agglomerative Clustering
Es una técnica de clustering jerárquico que construye la estructura de los clusters de forma ascendente (bottom-up):  
comienza con cada punto como un cluster separado y los va fusionando progresivamente según su similitud.  
- No requiere especificar una estructura rígida
- Se puede representar como un dendrograma
- Puedes definir el número de clusters deseado o un umbral de distancia

✅ **¿Cuándo usar Agglomerative Clustering?**
- Quieres una representación jerárquica de los datos
- No estás seguro del número óptimo de clusters
- Trabajas con datasets pequeños o medianos donde puedes visualizar estructuras de agrupación

## Mean Shift
Agrupa datos localizando zonas de alta densidad y desplazando puntos hacia los picos de densidad más cercanos.  
- No requiere definir el número de clusters.
- Detecta automáticamente la cantidad de grupos
- Identifica centros de densidad como centroides
- Es más lento que KMeans, pero más flexible

✅ **¿Cuándo usar Mean Shift?**
- Quieres detectar agrupaciones suaves y de forma variable
- No sabes cuántos clusters hay de antemano
- Trabajas con datos donde los grupos se distribuyen en densidades irregulares

## OPTICS
Es un algoritmo basado en densidad (como DBSCAN), pero mejora su capacidad para manejar clusters con diferentes densidades.  
- No produce directamente una asignación de clusters, sino un ordenamiento de alcance que se puede usar para construir agrupaciones.
- No necesita definir el número de clusters
- Es más robusto que DBSCAN en casos con densidades variables
- Identifica outliers y estructura interna de agrupación

✅ **¿Cuándo usar OPTICS?**
- Quieres detectar grupos en datos con densidades heterogéneas
- DBSCAN no entrega buenos resultados
- Quieres una alternativa flexible y explicativa

## Birch
Es un algoritmo diseñado para grandes volúmenes de datos, que realiza clustering de manera jerárquica y en tiempo eficiente.  
- Crea un árbol compacto (CF Tree) para representar los datos antes de aplicar un algoritmo final (como KMeans).
- Escala muy bien con datasets grandes
- Agrupa eficientemente en memoria limitada
- Permite procesar datos por lotes

✅ **¿Cuándo usar Birch?**
- Tienes un dataset muy grande o en streaming
- Quieres usar clustering jerárquico con bajo consumo de memoria
- Usas clustering como paso previo a otro algoritmo más fino



