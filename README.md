# 📊 Telecom X - Análisis de Evasión de Clientes (Churn)

## 📝 Descripción del Proyecto
Este proyecto forma parte del Challenge 2 de Data Science de Alura Latam y Oracle Next Education. El objetivo es analizar una base de datos de la empresa de telecomunicaciones "Telecom X" para identificar los factores principales que están provocando la alta tasa de cancelación de servicios (Churn) por parte de los clientes.

## 🛠️ Tecnologías y Herramientas
* **Python 3**
* **Pandas:** Para limpieza, aplanado de datos JSON (ETL) y manipulación de DataFrames.
* **Matplotlib y Seaborn:** Para el Análisis Exploratorio de Datos (EDA) y visualizaciones.
* **Google Colab:** Entorno de desarrollo.

## 🚀 Proceso Realizado (ETL y EDA)
1. **Extracción:** Carga de datos directamente desde una API REST en formato JSON y aplanado de estructuras anidadas.
2. **Transformación:** Limpieza de datos nulos, conversión de tipos de datos, creación de la variable `Cuentas_Diarias` y estandarización de la variable objetivo binaria `Churn_Binario`.
3. **Análisis:** Generación de métricas de correlación y visualización de perfiles de riesgo mediante gráficos de pastel, barras y mapas de calor.

## 💡 Conclusiones Principales
El análisis demostró que el mayor riesgo de evasión se concentra en los clientes que poseen **contratos de formato "Mes a mes" (Month-to-month)**. Aquellos clientes que logran ser migrados a contratos de 1 o 2 años presentan tasas de retención extremadamente altas. Además, se identificó una correlación directa entre el aumento del cargo mensual y la probabilidad de abandonar la compañía.
