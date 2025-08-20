TelecomX_part_2
📊 Predicción de Cancelación de Clientes - Telecom X
Este proyecto forma parte del desafío de ciencia de datos Telecom X, cuyo objetivo es prever qué clientes tienen mayor probabilidad de cancelar sus servicios. Se desarrolla un pipeline de machine learning desde la carga y limpieza de datos hasta la creación y evaluación de modelos predictivos, con visualizaciones e interpretaciones estratégicas.

🧠 Objetivo del Análisis
Anticipar la cancelación de clientes mediante modelos de clasificación, identificar los factores clave que impulsan esta decisión y proponer estrategias de retención efectivas basadas en datos.

🛠 Herramientas y Librerías
Python 3
pandas, numpy
matplotlib, seaborn, plotly
sklearn: modelos, métricas y preprocesamiento
imblearn: SMOTE para balanceo de clases
Google Colab para ejecución
GitHub para documentación y publicación
📁 Estructura del Proyecto
1. Carga y Preprocesamiento
Carga del archivo TelecomX_Data.json
Normalización de la estructura anidada
Conversión de datos numéricos y limpieza de nulos
Eliminación de columnas irrelevantes (customerID)
Codificación de variables categóricas (One-Hot Encoding)
2. Análisis Exploratorio
Análisis de correlación con la variable objetivo (Churn)
Visualización de relaciones clave:
Tenencia vs Cancelación
Gasto total vs Cancelación
Tipo de contrato vs Cancelación
3. Balanceo de Clases
Aplicación de SMOTE para abordar el desbalance entre clases (Churn: Yes / No)
4. Normalización de Datos
Aplicación de StandardScaler para modelos basados en distancia (Logistic Regression, KNN)
5. Modelado Predictivo
División del dataset en 80% entrenamiento / 20% prueba
Modelos implementados:
Regresión Logística (requiere normalización)
Random Forest (no requiere normalización)
Evaluación de desempeño con:
Accuracy
Precision
Recall
F1-score
Matriz de confusión
6. Interpretación de Resultados
Análisis de coeficientes (Regresión Logística)
Importancia de variables (Random Forest)
Comparación de modelos
Identificación de factores clave
📋 Conclusiones Estratégicas
Las principales variables asociadas a la cancelación son:
Tipo de contrato (Month-to-month)
Forma de pago (Electronic check)
Tenencia baja (poca antigüedad)
Gasto total acumulado
✅ Recomendaciones de Retención
Promover contratos a largo plazo con beneficios adicionales.
Detectar clientes con baja antigüedad y ofrecer incentivos de permanencia.
Mejorar experiencia de pago y automatización con métodos más estables.
Realizar campañas personalizadas hacia segmentos con mayor riesgo.
📂 Archivos del Repositorio
TelecomX_Churn_Analysis.ipynb: Notebook con el análisis completo.
TelecomX_Data.json: Dataset base (preprocesado desde la parte 1 del desafío).
README.md: Este archivo.
✨ Autor
Desarrollado por Daniel Gustavo Fernandez como parte del programa de formación en ciencia de datos 2025.

📈 Futuras Mejoras
Añadir modelos adicionales como KNN, SVM, XGBoost
Ajustar hiperparámetros con GridSearchCV
Implementar validación cruzada
Automatizar el pipeline en producción
Conectar con dashboards para monitoreo en tiempo real
