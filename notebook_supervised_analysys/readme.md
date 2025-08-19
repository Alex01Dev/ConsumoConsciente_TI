# Analisis Supervisado (Machine Learning)

<HR>

### Propuesta de la Aplicacion---
El objetivo es predecir el monto total de las compras de los usuarios basado en sus hábitos de consumo registrados en la tabla Purchase.

### Eleccion del mecanismo a utilizar
Se utilizará Regresión Lineal como algoritmo supervisado porque:

Nos servira para determinar el monto de cada compra: total_amount de cada compra.

Nos ayudara a predecir valores numéricos basados en atributos de entrada como: user_id, category_id, quantity, day_of_week, etc.

Mecanismo: Regresión Lineal Múltiple

### Marco Teorico
Regresión Lineal

La Regresión Lineal es un algoritmo supervisado utilizado para predecir valores continuos. Se basa en la relación lineal entre una variable dependiente (objetivo) y una o varias variables independientes (predictoras).

Fórmula General

y=β0​+β1​x1​+β2​x2​+⋯+βn​xn​+ϵ

Donde:
y = variable objetivo (total_amount)
x1​,x2​,...xn = variables predictoras (por ejemplo: quantity, category_id, day_of_week)
β0 = intercepto
β1,...,βn = coeficientes que representan la influencia de cada variable
ϵ = error aleatorio

### Aplicacion del Mecanismo
import pandas as pd
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score

##### Cargar dataset generado en ETL
dataset = pd.read_csv("purchase_dataset.csv")

##### Cargar predicciones generadas por el modelo
predictions = pd.read_csv("purchase_predictions.csv")

##### Variables reales y predichas
y_true = predictions["true_label"]
y_pred = predictions["pred_label"]

##### Calcular métricas de desempeño
accuracy = accuracy_score(y_true, y_pred)
precision = precision_score(y_true, y_pred, zero_division=0)
recall = recall_score(y_true, y_pred, zero_division=0)
f1 = f1_score(y_true, y_pred, zero_division=0)

print("📊 Resultados del modelo supervisado")
print(f"Accuracy  : {accuracy:.2f}")
print(f"Precision : {precision:.2f}")
print(f"Recall    : {recall:.2f}")
print(f"F1-Score  : {f1:.2f}")

### Graficos Generados (3 minimo)
Generacion y visualizacion de graficos relacionados con el analisis
supervisado

### Resultados Obtenidos
El modelo de análisis supervisado aplicado sobre la tabla de purchases alcanzó un rendimiento perfecto, con métricas de:

Accuracy: 1.0

Precision: 1.0

Recall: 1.0

F1-Score: 1.0

Esto significa que el modelo logró clasificar correctamente todos los registros sin errores. En el contexto del proyecto, indica que los datos de compras fueron predichos de manera totalmente precisa, lo cual demuestra un desempeño excelente del algoritmo en este conjunto de datos.

### Conclusion de la Fase del Proyecto
La implementación del análisis supervisado en nuestro proyecto permitió comprobar la eficacia de los algoritmos aplicados al conjunto de datos generado en la fase ETL. Los resultados obtenidos (accuracy, precision, recall y F1-score con valores de 1.0) evidencian que el modelo logró un desempeño óptimo, clasificando correctamente todos los registros sin errores.