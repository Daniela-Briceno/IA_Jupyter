# Aprendizaje Supervisado
Es un tipo de aprendizaje automático (Machine Learning) en el que un modelo aprende a partir de datos etiquetados, es decir:
- A cada entrada (input) se le asigna una salida conocida (output).
- El objetivo es que el modelo aprenda la relación entre los inputs y los outputs para poder predecir resultados en datos nuevos.

## Regresion lineal
Es un modelo estadístico que busca encontrar la relación lineal entre una variable independiente (X) y una dependiente (Y).  
Se representa con la fórmula: **Y = aX + b**  
Donde:  
- **a** es la pendiente (cuánto cambia Y si X cambia)
- **b** es la ordenada al origen (valor de Y cuando X = 0)  
✅ Se usa para predecir valores o detectar tendencias.

## Regresión logística

Es un modelo de clasificación que predice la probabilidad de que una observación pertenezca a una clase.  
A diferencia de la regresión lineal, su salida es una **probabilidad entre 0 y 1**, que se transforma en una clase (0 o 1).

Se representa con la función sigmoide:

**P(Y = 1 | X) = 1 / (1 + e^(-z))**  
Donde:  
- **z = aX + b** (igual que en regresión lineal)  
- **e** es el número de Euler (~2.718)  
- **a** son los coeficientes, y **b** es el sesgo

El modelo predice la clase final usando un umbral (por defecto: 0.5):  
- Si P ≥ 0.5 → clase 1  
- Si P < 0.5 → clase 0

✅ Se utiliza para clasificación binaria como:
- Diagnóstico médico (enfermo o sano)  
- Correo spam o no spam  
- Aprobación o rechazo de crédito

## Árbol de Decisión
Es un algoritmo de aprendizaje automático supervisado que se utiliza para **clasificación o regresión**.  
Funciona como un diagrama tipo árbol, donde cada nodo representa una decisión basada en los valores de las variables.

✅ **¿Cuándo usar un árbol de decisión?**
- Necesitas un modelo interpretable y fácil de explicar
- Trabajas con datos estructurados (columnas tipo Excel o base de datos)
- Tienes tanto variables categóricas como numéricas
- Quieres resolver problemas de clasificación o regresión
- No quieres preocuparte por la normalización o escalado de datos
- Tienes un dataset pequeño o mediano
- Necesitas saber por qué se llegó a cierta predicción  


## Random Forest
Es un algoritmo que combina múltiples árboles de decisión para mejorar la precisión y robustez del modelo.  
Funciona creando muchos árboles (generalmente entrenados con subconjuntos aleatorios de los datos) y tomando una decisión en conjunto:
- **Clasificación:** votación mayoritaria
- **Regresión:** promedio de predicciones  
Este enfoque reduce el overfitting, mejora la generalización y suele entregar mejor rendimiento que un solo árbol.  

✅ **¿Cuándo usar Random Forest?**
- Quieres mejorar la precisión respecto a un solo árbol de decisión
- Tienes datos estructurados con muchas variables
- Quieres un modelo robusto frente a ruido o overfitting
- Tienes tanto variables categóricas como numéricas
- Trabajas con un dataset pequeño o grande
- No necesitas un modelo tan fácil de interpretar como un árbol individual
- Buscas un buen desempeño sin mucho ajuste de hiperparámetros
