#  Retail Analytics Pipeline — Big Data con Apache Spark

##  Descripción

Este proyecto implementa un pipeline completo de Big Data utilizando Apache Spark para procesar datos de e-commerce, generar métricas de negocio y construir modelos de Machine Learning escalables.

Se trabaja con datos simulados de la empresa **RetailMax**, abordando desde el procesamiento distribuido hasta la generación de insights accionables para el área de marketing.

---

##  Objetivo

Diseñar un flujo analítico escalable que permita:

- Procesar grandes volúmenes de datos
- Generar métricas de negocio relevantes
- Identificar clientes de alto valor
- Segmentar usuarios según comportamiento
- Apoyar la toma de decisiones en marketing

---

##  Tecnologías utilizadas

- Python
- Apache Spark (PySpark)
- Spark SQL
- MLlib
- Matplotlib

---

##  Componentes del pipeline

###🔹 Procesamiento distribuido (RDDs)
- Transformaciones: `map`, `filter`, `reduceByKey`, `flatMap`, `distinct`, `sortBy`
- Acciones: `count`, `take`, `sum`, `mean`, `stdev`
- Evaluación perezosa (Lazy Evaluation)

### 🔹 Procesamiento estructurado
- DataFrames con esquema explícito (`StructType`)
- Consultas con Spark SQL
- Métricas de negocio:
  - ventas por categoría
  - comportamiento de clientes
  - análisis por región

### 🔹 Optimización
- Uso de `cache()` para evitar recomputación
- Documentación de linaje con `toDebugString()`

---

##  Machine Learning (MLlib)

### ✔ Regresión Logística (Supervisado)
- Clasificación de clientes de alto valor (`alto_valor`)
- Métricas:
  - AUC-ROC
  - Accuracy

### ✔ K-Means (No Supervisado)
- Segmentación de clientes en 3 clusters según comportamiento

### ✔ Variables utilizadas
- monto_final  
- paginas_vistas  
- tiempo_sesion  
- compras_previas  
- dias_sin_comprar  
- categoria_index  

---

##  Visualizaciones

Se incluyen gráficos para analizar:

- Ventas por categoría  
- Distribución de clientes premium  
- Comparación de gasto promedio  
- Nivel de engagement (páginas vistas)  

---

##  Resultados principales

- Identificación de clientes de alto valor mediante modelo predictivo  
- Segmentación de usuarios con perfiles diferenciados  
- Detección de patrones de comportamiento en navegación y compra  
- Generación de insights accionables para marketing  

---

##  Insights de negocio

- Clientes de alto valor permiten campañas personalizadas  
- Segmentos con bajo engagement requieren estrategias de retención  
- Clientes premium presentan mayor ticket promedio → oportunidades de upselling  
- Alta interacción digital se asocia a mayor probabilidad de conversión  

---


---

##  Nota técnica

La persistencia en formato **Parquet** no fue ejecutada debido a restricciones de configuración de Hadoop en entorno local Windows.  
Sin embargo, el diseño del pipeline contempla su implementación en entornos productivos distribuidos.

---

##  Autor

**Carolina Tapia Bahamonde**  
Ingeniera Civil en Informática  
Especialización en Ciencia de Datos  

---

##  Contexto académico

Proyecto desarrollado en:

**Fundamentos de Big Data — Módulo 9**  
Programa de Especialización en Ciencia de Datos  
Talento Digital / Pixelab
