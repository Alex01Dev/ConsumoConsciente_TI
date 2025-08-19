# Proceso ETL (Extracción, Transformación, Carga)
<HR>

## Importación de Librerias
import numpy as np #Sirve par apoder ealizar procesamientos basicos numericos de datos cuantitativos
import pandas as pd #Sirve para reutilizar los procesos ETL en un conjunto de Datos
import time #Sirve para la manipulacion de datos en diferentes formatos de tiempo

### Graficadores (Plots)

import matplotlib.pyplot as plt #Librería base para gráficos en 2D.
import plotly.express as px #Se usa mucho para análisis estadístico visual.
import seaborn as sns #Para gráficos interactivos y dinámicos.

## Carga de Datos
!cd
!dir

## Creación de Dataframe
df = pd.read_csv('products.csv', encoding="latin1")

print(type(df)) # Corroboramos tipo de dato en nuestro objeto

## Analisis Exploratorio de los datos (EDA)
print(type(df)) # Corroboramos tipo de dato en nuestro objeto

df.describe() ## Realiza un reporte estadisticos sobre columnas completamente numericos (cuantitativos)

df.isnull() ## Mapea la matriz original con una matriz



## Limpieza de Datos
df_duplicados_eliminados= df.drop_duplicates() ## Este metodo elimina los datos duplicados en base al criterio de la totalidad de los datos, esto se debe realizar
                    ## con extrema cautela dato que si no se tiene un atributo indentificar se alteraran resultados esperados

df_duplicados_eliminados.info()

df_vacios_eliminados= df.dropna()

df_vacios_eliminados.info()

print("DataFrame Original:")
print(len(df))
print("DataFrame sin datos nulos en la columna:")
print(len(df_vacios_eliminados))

## Visualización de Datos (2 a 5 gráficas)
### --- 1. Estatus disponible vs agotado ---
status_counts = df['status'].value_counts()

status_counts.plot(kind="bar", edgecolor="black")
plt.title("Disponibilidad de productos")
plt.xlabel("Estatus")
plt.ylabel("Cantidad")
plt.show()

### --- 2. Distribución de huella de carbono ---
plt.hist(df['carbon_footprint'], bins=10, color="green", edgecolor="black")
plt.title("Distribución de productos por huella de carbono")
plt.xlabel("Huella de carbono")
plt.ylabel("Cantidad de productos")
plt.show()

## Exportación de data SET (.csv)
df.to_csv("products_export.csv", index=False, encoding="utf-8")

## Conclusión de esta Fase

Este trabajo nos permitió desarrollar nuevas habilidades y aplicar de manera práctica lo aprendido en clase. La manipulación de datos algo complejos mediante un ETL representó un reto, al igual que la implementación de análisis supervisados y no supervisados. Consideramos que fue un proyecto que puso a prueba nuestras capacidades y que logramos completar de manera satisfactoria.