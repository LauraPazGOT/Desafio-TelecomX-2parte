# Desafio-TelecomX-2parte
Predicción de cancelación de clientes en telecomunicaciones mediante análisis de datos y modelos de machine learning.

📊 Predicción de Cancelación de Clientes (Churn) — Telecom X
📌 Descripción del proyecto

Este proyecto tiene como objetivo analizar los factores asociados a la cancelación de clientes en una empresa de telecomunicaciones y desarrollar modelos de machine learning capaces de predecir qué clientes tienen mayor probabilidad de abandonar el servicio.

El análisis se basa en datos reales proporcionados por Telecom X e incluye etapas de exploración, preparación de datos, modelado predictivo e interpretación de resultados con enfoque estratégico.

🎯 Objetivos

Identificar los factores que influyen en la cancelación de clientes.

Preparar los datos para modelado predictivo.

Entrenar y evaluar distintos modelos de clasificación.

Interpretar la importancia de las variables.

Proponer insights aplicables al negocio.

🧰 Tecnologías utilizadas

Python

Pandas

NumPy

Matplotlib / Seaborn

Scikit-learn

Google Colab

📂 Etapas del proyecto
1️⃣ ETL y Análisis Exploratorio

Extracción de datos desde JSON.

Limpieza y transformación.

Análisis descriptivo.

Identificación de patrones de churn.

2️⃣ Preparación de Datos

Codificación de variables categóricas.

Normalización de variables numéricas.

Separación en datos de entrenamiento y prueba.

3️⃣ Modelado Predictivo

Se entrenaron tres modelos:

Regresión Logística

Árbol de Decisión

Random Forest

Los modelos fueron evaluados utilizando métricas como:

Accuracy

Precision

Recall

F1-Score

🏆 Resultados

El modelo de Regresión Logística presentó el mejor desempeño para este problema, destacándose especialmente en la detección de clientes en riesgo de cancelación (mayor recall).

Esto es particularmente importante en problemas de churn, donde el objetivo principal es anticipar qué clientes podrían abandonar el servicio.

🔍 Principales hallazgos

El análisis permitió identificar factores clave asociados al churn:

Los clientes con menor antigüedad presentan mayor riesgo de cancelación.

Los contratos mensuales muestran mayor tasa de abandono.

Los cargos mensuales elevados se asocian con mayor churn.

La ausencia de servicios adicionales reduce la fidelización.

🧠 Interpretación para el negocio

Los resultados sugieren que las estrategias de retención deberían enfocarse principalmente en:

Clientes nuevos

Usuarios con contratos mensuales

Clientes sin servicios complementarios

Clientes con altos costos mensuales

Estas acciones podrían reducir significativamente la tasa de cancelación.

⚙️ Mejoras implementadas

Este proyecto fue mejorado progresivamente aplicando buenas prácticas de machine learning y validación profesional de modelos:

Split estratificado de datos
Se utilizó stratify=y en la separación de entrenamiento y prueba para preservar la proporción real de churn en ambos conjuntos, evitando sesgos de evaluación.

Modelo baseline (Dummy Classifier)
Se incorporó un modelo de referencia que predice la clase más frecuente, permitiendo verificar que los modelos entrenados superan significativamente una predicción trivial.

Escalado correcto de variables numéricas
Se aplicó StandardScaler ajustado únicamente sobre el conjunto de entrenamiento, evitando data leakage y asegurando una evaluación válida.

Optimización del modelo final
Se mejoró la Regresión Logística utilizando class_weight="balanced" para compensar el desbalance de clases, aumentando significativamente la capacidad de detección de clientes en riesgo (recall).

Comparación sistemática de modelos
Se evaluaron múltiples algoritmos (Regresión Logística, Árbol de Decisión y Random Forest) utilizando métricas clave para problemas de churn:

Recall (prioritario para retención)

Precision

F1-score

Accuracy

Interpretación de variables relevantes
Se analizó la importancia de las variables mediante:

coeficientes de Regresión Logística

feature importance de Random Forest

Esto permitió identificar factores clave de cancelación desde una perspectiva de negocio.

Enfoque orientado a aplicación real
El modelo final fue seleccionado priorizando la capacidad de detectar clientes en riesgo, alineado con objetivos reales de retención en telecomunicaciones.


📁 Estructura del repositorio
├── DesafioTelecomX2parte.ipynb
├── datos_tratados.csv
└── README.md

🚀 Autor

Proyecto desarrollado por Laura Paz como parte del desafío de Ciencia de Datos — Alura LATAM.

⭐ Nota final

Este proyecto demuestra cómo la ciencia de datos puede aplicarse para resolver problemas reales del negocio, permitiendo anticipar riesgos, optimizar decisiones y mejorar la retención de clientes.

