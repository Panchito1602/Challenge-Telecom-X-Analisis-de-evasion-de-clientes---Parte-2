# 📉 Telecom X: Predicción de Cancelación de Clientes (Churn)

---

## 📖 Descripción del Proyecto
Este proyecto forma parte del Challenge "Telecom X" propuesto por **Alura Latam**. Asumiendo el rol de Analista Junior de Machine Learning, el objetivo principal es desarrollar un pipeline predictivo capaz de anticipar qué clientes tienen mayor probabilidad de cancelar sus servicios (*Churn*). 

A través del procesamiento de datos, análisis de correlación y entrenamiento de modelos de clasificación, se busca no solo predecir la fuga, sino también entregar *insights* estratégicos y accionables para la retención de clientes.

---

## 🎯 Objetivos
* **Preprocesamiento de datos:** Limpieza, One-Hot Encoding y Estandarización de variables numéricas.
* **Balanceo de Clases:** Aplicación de SMOTE (Synthetic Minority Over-sampling Technique) en los datos de entrenamiento para abordar el desbalance de la variable objetivo.
* **Análisis Exploratorio y Correlación:** Identificación de las variables con mayor peso en la decisión de cancelación del cliente.
* **Modelado Predictivo:** Entrenamiento y evaluación de modelos de **Regresión Logística** y **Random Forest**.
* **Estrategia de Negocio:** Traducción de métricas técnicas a un informe ejecutivo con recomendaciones viables.

---

## 🛠️ Tecnologías y Librerías Utilizadas
* **Lenguaje:** Python
* **Manipulación de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Logistic Regression, RandomForestClassifier, StandardScaler, métricas de evaluación)
* **Balanceo de Datos:** Imbalanced-learn (SMOTE)

---

## 🚀 Resultados Destacados

### Desempeño de los Modelos
Se evaluaron dos modelos contrastantes. El modelo ganador fue la **Regresión Logística**, destacando por su capacidad de generalización y mejor identificación de los casos positivos de Churn:
* **Exactitud (Accuracy):** 79.70%
* **Sensibilidad (Recall):** 54.72%
* **F1-Score:** 0.5887
* *Nota:* El modelo Random Forest presentó señales de *overfitting* (87.5% en Train vs 79.4% en Test), mientras que la Regresión Logística mantuvo un rendimiento estable y sin sesgos de sobreajuste.

### Insights de Negocio (Drivers de Churn)
El análisis de importancia de variables y correlaciones reveló tres grandes áreas de mejora:
1. **El Riesgo de la Fibra Óptica:** Los clientes con este servicio presentan la mayor probabilidad de abandonar la empresa, lo que sugiere problemas técnicos o de competitividad en precios.
2. **Fricción en Pagos:** El uso de Cheque Electrónico (*Electronic check*) está altamente correlacionado con el churn.
3. **Contratos Cortos:** Los clientes sin contratos a largo plazo y con facturaciones altas son altamente volátiles. La antigüedad en la empresa es el mayor factor protector.

## 💡 Recomendaciones Estratégicas
* Realizar una auditoría técnica y comercial urgente sobre el servicio de Fibra Óptica.
* Implementar campañas para migrar a los clientes del Cheque Electrónico hacia el débito automático.
* Ofrecer incentivos de fidelidad (upselling) durante los primeros 6 meses para asegurar contratos anuales o bianuales.

---

## 👤 Autor
**Luis Alejandro Mamani Garnique** *Estudiante de Ingeniería Industrial en la UNMSM (8vo ciclo).* *Estudiante del grupo G9 ORACLE NEXT GENERATION.* *Practicante de Gestión y Control de Información en el área de Operaciones.* *Interesado en la Ciencia de Datos y la Analítica aplicada a la optimización de procesos.*

---

## 🚀 Instrucciones para Ejecutar
1. Clonar el repositorio: `git clone https://github.com/Panchito1602/Alura-Latam-DataScience-Challenge-1`
2. Abrir el archivo `.ipynb` en **Google Colab**.
3. Ejecutar las celdas en orden para cargar los datasets desde el repositorio de Alura y visualizar los gráficos generados.
