# 📊 Telecom X – Análisis de Evasión de Clientes

## 🎯 Objetivo

Este proyecto tiene como propósito **analizar los datos históricos de clientes de Telecom X** para comprender los factores que influyen en la evasión (churn).  
A través de un proceso de **limpieza, transformación y análisis exploratorio de datos**, se buscó:

- Identificar patrones asociados al abandono de clientes.  
- Extraer **insights accionables** para diseñar estrategias de retención.  
- Generar insumos que faciliten la construcción de **modelos predictivos de churn**.  

---

## 🧠 Habilidades practicadas

Durante el desarrollo se aplicaron competencias clave de Ciencia de Datos:

- Gestión de datos estructurados en formato JSON.  
- Proceso **ETL** (Extracción, Transformación y Carga).  
- Análisis exploratorio de datos (**EDA**) con visualizaciones significativas.  
- Tratamiento de datos faltantes y detección de incoherencias.  
- Normalización de variables categóricas y numéricas.  
- Evaluación de correlaciones entre variables.  
- Elaboración de un informe final claro, estructurado y documentado.  

---

## 📂 Flujo del análisis

### 🔹 Extracción
- Se cargaron archivos JSON con información de clientes, servicios contratados y facturación.  

### 🔹 Transformación

#### ✅ Exploración inicial
- Inspección de columnas, estructura y tipos de datos.  
- Uso de un diccionario de datos para interpretar cada variable.  

#### ✅ Detección y corrección de incoherencias
- Identificación de valores nulos en campos como `cargo_total`.  
- Eliminación o imputación de registros incompletos.  

#### ✅ Creación de nuevas variables
- `cargo_diario`: cargo mensual dividido entre 30.  
- `cantidad_servicios`: suma de los servicios contratados por cliente.  

#### ✅ Estandarización
- Columnas renombradas a español con formato `snake_case`.  
- Variables binarias (`Yes/No`) convertidas a numéricas (`1/0`).  

---

### 🔹 Carga y análisis

#### 📈 Estadísticos descriptivos
- Uso de `.describe()` para variables numéricas clave.  

#### 📉 Distribución de churn
- Gráfico de barras para visualizar la proporción de clientes que abandonan vs. permanecen.  

#### 🧩 Churn por variables categóricas
- Agrupación por `tipo_contrato`, `metodo_pago`, `pareja`, etc.  
- Visualización de la proporción de abandono en cada categoría.  

#### 📊 Variables numéricas vs. churn
- Boxplots para `meses_contrato`, `cargo_total` y `cargo_diario`.  

#### 🔍 Correlaciones
- Matriz de correlación y heatmap.  
- Se encontró que `meses_contrato` y `cantidad_servicios` tienen fuerte relación **negativa** con la evasión.  

---

### 🔹 Informe Final
- Redactado en el archivo `.ipynb`.  
- Incluye: introducción, limpieza, análisis, visualizaciones y conclusiones.  

---

## 📊 Visualizaciones incluidas
- Gráficos de barras (churn total).  
- Gráficos apilados (categóricas vs. churn).  
- Boxplots (numéricas vs. churn).  
- Heatmap de correlaciones.  

Todas integradas y comentadas en el notebook.
