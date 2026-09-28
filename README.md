# Visualización de Datos: Análisis Comercial y Tendencias

Este repositorio contiene una serie de proyectos de análisis exploratorio y visualización de datos orientados a la toma de decisiones. A través del uso avanzado de herramientas de inteligencia de negocios, se abordan problemas reales de distribución espacial, tendencias temporales y correlación de variables.

## Tecnologías y Herramientas Utilizadas
* **Herramienta Principal:** Tableau Desktop
* **Conceptos Aplicados:** Pequeños múltiplos (Small Multiples), Cálculos de tabla rápidos (Promedios móviles), Análisis de correlación lineal, Ejes duales y Mapas espaciales.

---

## Proyectos Incluidos

### 1. Análisis Espacial de Rendimiento Comercial (Dataset: Superstore)
**Objetivo:** Evaluar la evolución de la rentabilidad y el volumen de ventas en distintas ciudades a lo largo del tiempo, desglosado por año y categoría de producto.
* **Técnica visual:** Visualización de pequeños múltiplos (Small Multiples) geográficos. Se codificó el volumen de ingresos mediante el tamaño de las marcas y la rentabilidad mediante la intensidad del color.
* **Hallazgos Clave:** 
  * **Evolución de Tecnología:** Se observa una evolución positiva en la distribución espacial de las ventas y ganancias. Hacia 2023, aparecen marcas de mayor tamaño en diferentes ciudades, representando un aumento en ingresos. A la par, hay una mayor presencia de tonalidades verdes que indican ganancias altas. Sin embargo, persisten algunas ciudades con tonalidades rojas, demostrando que el crecimiento de ventas no implica rentabilidad uniforme.
  * **Categoría Crítica (Furniture):** Presenta ciudades con un volumen de ventas considerable (marcas grandes) pero con tonalidades rojas o anaranjadas. Esto evidencia una brecha importante entre la distribución de ingresos y la rentabilidad, ya que el alto volumen de transacciones no se está traduciendo en ganancias.

### 2. Análisis de Tendencias en Seguridad Aérea (Dataset: LifePlane)
**Objetivo:** Identificar el patrón temporal de incidentes y accidentes aéreos a lo largo de varias décadas, mitigando el ruido de las fluctuaciones anuales.
* **Técnica visual:** Gráfico de líneas de series temporales con eje dual, superponiendo el recuento de eventos con un cálculo de promedio móvil (ventana de 2 periodos anteriores).
* **Hallazgos Clave:**
  * Al aislar el ruido anual, se descubrió un crecimiento sostenido de eventos en la aviación que alcanzó su pico histórico entre 2010 y 2012.
  * Al desglosar por tipo de evento (`Accident` vs `Incident`), se demostró que la tasa de accidentes se ha mantenido estable históricamente. El pico global fue impulsado exclusivamente por un aumento masivo en el volumen de reporte de incidentes menores a partir de 2005.

### 3. Impacto del Marketing en Ingresos (Dataset: Marketing)
**Objetivo:** Demostrar a la dirección general el retorno de inversión (ROI) de las campañas publicitarias en televisión durante los últimos 20 meses.
* **Técnica visual:** Gráfico de dispersión (Scatter plot) con línea de tendencia lineal. 
* **Hallazgos Clave:**
  * Existe una clara correlación positiva entre el número de anuncios emitidos y los ingresos generados.
  * La inversión recurrente se concentró entre 20 y 30 anuncios, manteniendo los ingresos estables. No obstante, se identificó un mes con valores atípicos positivos (35 anuncios) donde los ingresos superaron los $77,000 USD, alejándose hacia arriba de la línea de tendencia central e indicando un rendimiento excepcional.

---

## Estructura del Repositorio
* `/data/`: Contiene los conjuntos de datos originales (`Sample-Superstore.xls`, `lifeplane.csv`, `marketing.csv`).
* `/visualizations/`: Imágenes exportadas de los tableros, mapas y gráficos generados en Tableau.

---

