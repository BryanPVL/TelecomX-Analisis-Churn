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
---

## 🤖 Parte 2: Machine Learning y Modelos Predictivos (NUEVO)
En la segunda fase de este proyecto, asumí el rol de Data Scientist para construir modelos de predicción capaces de anticiparse a la fuga de clientes.

### 🛠️ Técnicas Aplicadas
* **Preprocesamiento:** One-Hot Encoding para variables categóricas.
* **Balanceo de Clases:** Implementación de la técnica **SMOTE** para equilibrar el conjunto de datos de entrenamiento y evitar sesgos hacia la clase mayoritaria.
* **Modelado:** Entrenamiento y evaluación de algoritmos de **Regresión Logística** (con normalización StandardScaler) y **Random Forest**.

### 📊 Resultados y Predicciones
El análisis de importancia de características (Feature Importance) del modelo Random Forest confirmó que las variables con mayor poder predictivo de cancelación son:
1. **Tipo de Contrato:** Los clientes con modalidad "Month-to-month" (mes a mes) representan el mayor riesgo de fuga.
2. **Tiempo de Permanencia (Tenure):** El riesgo de cancelación es crítico durante los primeros meses del ciclo de vida del cliente.
3. **Cargos Económicos:** Facturaciones totales altas sin la protección de un contrato a largo plazo aceleran la evasión.

**📁 Entregable Adicional:** Se adjunta en este repositorio el archivo `Reporte_Ejecutivo_TelecomX.pdf` generado dinámicamente con Python (`fpdf`), el cual contiene las métricas visuales y las recomendaciones estratégicas para el equipo de retención.
