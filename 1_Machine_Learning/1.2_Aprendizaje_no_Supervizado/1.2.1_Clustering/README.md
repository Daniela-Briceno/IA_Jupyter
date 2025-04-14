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



