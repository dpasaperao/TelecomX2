TelecomX_part_2

📊 Predicción de Abandono de Clientes - Telecom X

Este trabajo corresponde al reto de ciencia de datos Telecom X, cuyo propósito es anticipar qué usuarios tienen mayor posibilidad de dar de baja sus servicios. Se implementa un flujo completo de machine learning que abarca desde la carga y depuración de la información hasta la construcción y validación de modelos predictivos, acompañado de visualizaciones y conclusiones estratégicas.

🧠 Meta del Estudio

Predecir la deserción de clientes mediante algoritmos de clasificación, descubrir los factores determinantes de dicha conducta y plantear tácticas de retención fundamentadas en datos.

🛠 Tecnologías y Librerías Utilizadas
Python 3
pandas, numpy
matplotlib, seaborn, plotly
sklearn: algoritmos, métricas y preprocesamiento
imblearn: SMOTE para balancear clases
Google Colab para la ejecución
GitHub para registro y difusión

📁 Organización del Proyecto
Carga y Preparación de Datos
Lectura del archivo TelecomX_Data.json
Aplanamiento de estructura jerárquica
Conversión a formatos numéricos y tratamiento de valores nulos
Eliminación de campos no útiles (customerID)
Codificación de variables categóricas (One-Hot Encoding)
Exploración de Datos
Revisión de correlaciones con la variable objetivo (Churn)
Visualización de relaciones principales:
Tiempo de permanencia vs Abandono
Gasto acumulado vs Abandono
Tipo de contrato vs Abandono
Balanceo de Clases
Uso de SMOTE para corregir el desbalance entre clientes que cancelan y los que no.
Normalización
Escalado con StandardScaler para algoritmos sensibles a la distancia (Regresión Logística, KNN).
Modelado Predictivo
Separación del dataset: 80% entrenamiento / 20% prueba
Algoritmos utilizados:
Regresión Logística (requiere normalización)
Random Forest (sin necesidad de normalización)
Métricas de evaluación:
Accuracy
Precision
Recall
F1-score
Matriz de confusión
Análisis de Resultados
Estudio de coeficientes (Regresión Logística)
Importancia de variables (Random Forest)
Comparación de rendimiento entre modelos
Identificación de factores influyentes

📋 Conclusiones Clave
Las variables más relacionadas con la cancelación son:
Contratos mensuales (Month-to-month)
Método de pago (Electronic check)
Baja permanencia en la empresa
Monto acumulado de gasto

✅ Estrategias de Retención Propuestas
Incentivar contratos de mayor duración con beneficios exclusivos.
Detectar clientes con poca antigüedad y ofrecer promociones de fidelización.
Optimizar la experiencia de pago con métodos más confiables.
Lanzar campañas dirigidas a los segmentos con mayor probabilidad de abandonar.

📂 Archivos en el Repositorio
TelecomX_Churn_Analysis.ipynb: notebook con el análisis completo
TelecomX_Data.json: dataset base (procesado en la primera parte del reto)
README.md: archivo de documentación

✨ Autoría
Proyecto desarrollado por David Alonso Pasapera Obando - Ciencia de Datos 2025

📈 Próximos Avances
Implementar más algoritmos: KNN, SVM, XGBoost
Ajustar parámetros con GridSearchCV
Incorporar validación cruzada
Automatizar el flujo en un entorno productivo
Integrar dashboards para monitoreo en tiempo real
