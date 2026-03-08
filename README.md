# 🤖 Telecom X - Parte 2: Predicción de Evasión (Machine Learning)

Este repositorio contiene la segunda fase del proyecto de Telecom X. Tras realizar el análisis exploratorio (EDA), el enfoque ahora se centra en la construcción, entrenamiento y evaluación de modelos de **Aprendizaje Automático (Machine Learning)** para predecir qué clientes tienen mayor probabilidad de cancelar sus servicios.





## 🎯 Objetivo de la Misión
Desarrollar un pipeline de inteligencia predictiva que permita a Telecom X anticiparse a la pérdida de clientes (*Churn*), identificando perfiles de riesgo y variables determinantes para implementar estrategias de retención personalizadas.

## 🛠️ Stack Tecnológico
- **Lenguaje:** Python 3.x
- **Librerías de ML:** - `Scikit-learn`: Implementación de algoritmos de clasificación y preprocesamiento.
  - `Pandas` & `Numpy`: Manipulación de datos y limpieza.
  - `Seaborn` & `Matplotlib`: Visualización de métricas y correlaciones.

## 🔄 Pipeline de Ciencia de Datos

### 1. Preprocesamiento de Datos
Para preparar los datos para los algoritmos, se realizaron las siguientes tareas:
- **Encoding:** Transformación de variables categóricas mediante *One-Hot Encoding*.
- **Limpieza de Identificadores:** Eliminación de columnas no predictivas (como IDs de cliente).
- **Escalamiento:** Normalización de características numéricas mediante `StandardScaler` para asegurar la convergencia de modelos lineales.

### 2. Modelado y Entrenamiento
Se implementaron y compararon dos enfoques distintos:
- **Regresión Logística:** Modelo lineal para establecer una base de comparación y entender coeficientes.
- **Random Forest:** Modelo basado en conjuntos de árboles para capturar relaciones no lineales complejas.

### 3. Evaluación de Rendimiento
Los modelos fueron evaluados bajo métricas rigurosas:
- **Recall (Sensibilidad):** Priorizado para minimizar los falsos negativos (clientes que se van y no detectamos).
- **Matriz de Confusión:** Para visualizar el balance de aciertos y errores.
- **Importancia de Variables:** Identificación de los 10 factores con mayor peso en la predicción.

---

## 📊 Hallazgos Principales
- **Factor Crítico:** El tipo de contrato (mensual vs. anual) sigue siendo el predictor más fuerte de abandono.
- **Relación de Servicios:** Los clientes de fibra óptica presentan una correlación atípica con la fuga, sugiriendo una oportunidad de mejora en la estabilidad o precio de este producto.
- **Punto de Retención:** El modelo detecta un riesgo máximo en clientes con menos de 12 meses de permanencia.



## 🚀 Cómo utilizar este Repositorio
1. Clona este repositorio.
2. Asegúrate de tener instaladas las dependencias: `pip install scikit-learn pandas seaborn matplotlib requests`.
3. Ejecuta el archivo `Challenge Alura Latam - TelecomX_LATAM- Parte 2`. El notebook consume automáticamente los datos tratados desde la API/GitHub.



---
> *Este proyecto es el resultado del Challenge Telecom X, integrando habilidades de Ingeniería de Datos y Ciencia de Datos aplicada al negocio.*
