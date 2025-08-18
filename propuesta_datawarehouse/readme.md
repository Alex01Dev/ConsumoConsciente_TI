
# Propuesta Data Warehouse

---

## Contexto de un Data Warehouse en el proyecto

Un **Data Warehouse (DW)** es un sistema de almacenamiento centralizado que permite integrar, organizar y analizar grandes volúmenes de información provenientes de múltiples fuentes. En el contexto de nuestra aplicación de **productos sustentables**, el DW servirá para consolidar datos de compras, usuarios, productos, proveedores y comportamiento de consumo, facilitando análisis avanzados y generación de reportes estratégicos para mejorar la toma de decisiones.

Los **orígenes de datos** principales relacionados con nuestro proyecto incluyen:

* **Datos transaccionales**: Información de las compras realizadas por los usuarios (productos comprados, cantidades, fecha).
* **Datos de usuarios**: Perfil del consumidor (edad, preferencias de productos).
* **Datos de productos**: Información de productos (categoría, huella de carbono, origen local, empaque reciclable).
* **Datos externos**: Información de tendencias de sostenibilidad, indicadores ambientales.

Estos datos se integran para generar una visión unificada del negocio, permitiendo identificar patrones de consumo y oportunidades de mejora.

---

## Propuesta de 3 orígenes de datos alternativos

1. **Plataformas de reseñas de productos**

   * Fuente: Sitios web que permiten calificar productos sustentables.
   * Utilidad: Permite evaluar la percepción del consumidor sobre los productos y enriquecer nuestro análisis de satisfacción y reputación.

2. **Datos de redes sociales**

   * Fuente: Comentarios, publicaciones y tendencias relacionadas con sostenibilidad en plataformas como Instagram, Twitter o TikTok.
   * Utilidad: Ayuda a identificar productos emergentes, preferencias de los consumidores y comportamientos de compra influenciados por tendencias sociales.

3. **Indicadores de impacto ambiental**

   * Fuente: Bases de datos públicas sobre huella de carbono, emisiones de CO₂ y certificaciones ecológicas.
   * Utilidad: Permite asociar datos de nuestros productos con su impacto ambiental, ayudando a los consumidores a tomar decisiones más conscientes y a la empresa a priorizar proveedores sostenibles.

---

## 5 Experimentos de asociación (mezcla) de datos

1. **Asociación de compras y perfil del usuario**

   * Objetivo: Analizar qué tipos de productos prefieren los distintos segmentos de usuarios ( hábitos).

2. **Asociación de productos y reseñas externas**

   * Objetivo: Correlacionar la calificación de los productos en plataformas externas con la frecuencia de compra interna.

3. **Asociación de redes sociales y tendencias de consumo**

   * Objetivo: Identificar si los productos populares en redes sociales generan un aumento en ventas dentro de la aplicación.

4. **Asociación de impacto ambiental y decisión de compra**

   * Objetivo: Determinar si los usuarios valoran la sostenibilidad al elegir productos.

5. **Asociación de proveedores y comportamiento de compra**

   * Objetivo: Analizar si ciertos proveedores generan mayor fidelización y qué características de sus productos influyen en la repetición de compra.

---

## Toma de decisiones

Supuestos estratégicos derivados de la integración de datos:

1. Los **usuarios que compran productos con menor huella de carbono** son más propensos a interactuar con promociones ecológicas.
2. La **mezcla de datos de reseñas externas y ventas internas** permitirá ajustar el catálogo de productos, eliminando aquellos con baja aceptación.
3. Los **patrones de comportamiento en redes sociales** pueden anticipar tendencias de consumo, ayudando a planificar campañas de marketing sostenibles.
4. Integrar **indicadores de impacto ambiental y compras** permitirá diseñar estrategias de fidelización, premiando a los consumidores conscientes.
5. La **comparación de proveedores y desempeño de ventas** permitirá optimizar la cadena de suministro priorizando proveedores sostenibles y confiables.
















