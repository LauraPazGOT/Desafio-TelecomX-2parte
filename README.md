📊 Predicción de Cancelación de Clientes (Churn) — Telecom X

Predicción de cancelación de clientes en telecomunicaciones mediante análisis de datos y modelos de machine learning.

📌 Descripción del proyecto

Este proyecto tiene como objetivo analizar los factores asociados a la cancelación de clientes en una empresa de telecomunicaciones y desarrollar modelos de machine learning capaces de predecir qué clientes tienen mayor probabilidad de abandonar el servicio.

El análisis incluye etapas de exploración de datos, preparación, modelado predictivo e interpretación de resultados con enfoque estratégico orientado al negocio.

🎯 Objetivos

Identificar los factores que influyen en la cancelación de clientes

Preparar los datos para modelado predictivo

Entrenar y evaluar distintos modelos de clasificación

Interpretar la importancia de las variables

Proponer insights aplicables al negocio

🧰 Tecnologías utilizadas

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Google Colab

📂 Etapas del proyecto
1️⃣ ETL y Análisis Exploratorio

Extracción de datos desde JSON

Limpieza y transformación

Análisis descriptivo

Identificación de patrones de churn

2️⃣ Preparación de Datos

Codificación de variables categóricas

Normalización de variables numéricas

Separación en datos de entrenamiento y prueba

3️⃣ Modelado Predictivo

Se entrenaron tres modelos:

Regresión Logística

Árbol de Decisión

Random Forest

Los modelos fueron evaluados utilizando métricas estándar:

Accuracy

Precision

Recall

F1-score

🏆 Resultados

El modelo de Regresión Logística balanceada presentó el mejor desempeño para este problema, destacándose especialmente en la detección de clientes en riesgo de cancelación (mayor recall).

Esto es especialmente relevante en problemas de churn, donde el objetivo principal es anticipar la cancelación y permitir acciones de retención.

🔍 Principales hallazgos

El análisis permitió identificar factores clave asociados al churn:

Clientes con menor antigüedad presentan mayor riesgo de cancelación

Contratos mensuales muestran mayor tasa de abandono

Cargos mensuales elevados se asocian con mayor churn

La ausencia de servicios adicionales reduce la fidelización

🧠 Interpretación para el negocio

Los resultados sugieren que las estrategias de retención deberían enfocarse en:

Clientes nuevos

Usuarios con contratos mensuales

Clientes sin servicios complementarios

Clientes con altos costos mensuales

Estas acciones podrían reducir significativamente la tasa de cancelación.

⚙️ Mejoras implementadas

Este proyecto fue optimizado aplicando buenas prácticas profesionales de machine learning:

Split estratificado de datos
Se utilizó stratify=y para preservar la proporción real de churn en train y test.

Modelo baseline (Dummy Classifier)
Se implementó un modelo de referencia para validar que los modelos entrenados aportan valor real.

Escalado correcto de variables numéricas
Se utilizó StandardScaler ajustado únicamente sobre el conjunto de entrenamiento, evitando data leakage.

Optimización del modelo final
Se aplicó class_weight="balanced" en la Regresión Logística, mejorando significativamente el recall de churn.

Comparación sistemática de modelos

Se evaluaron múltiples algoritmos utilizando métricas clave:

Recall

Precision

F1-score

Accuracy

Interpretación de variables relevantes

Se analizaron las variables más influyentes mediante:

coeficientes de Regresión Logística

feature importance de Random Forest

Enfoque orientado a negocio

El modelo final fue seleccionado priorizando la detección de clientes en riesgo, alineado con objetivos reales de retención.

📁 Estructura del repositorio
DesafioTelecomX2parte.ipynb
datos_tratados.csv
README.md
🚀 Autor

Laura Paz
Proyecto desarrollado como parte del desafío de Ciencia de Datos — Alura LATAM.

⭐ Conclusión

Este proyecto demuestra cómo la ciencia de datos puede aplicarse para resolver problemas reales de negocio, permitiendo anticipar cancelaciones, optimizar decisiones y mejorar la retención de clientes mediante modelos predictivos interpretables.
