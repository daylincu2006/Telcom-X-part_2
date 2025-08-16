📊 Challenge Telecom X: Análisis de Evasión de Clientes – Parte 2
🎯 Objetivo del Proyecto
Desarrollar y comparar modelos predictivos para identificar clientes con riesgo de evasión, maximizando el recall en la clase minoritaria (clientes que abandonan) 
sin comprometer excesivamente la precisión, y reduciendo el impacto de falsos positivos en decisiones comerciales.

🛠️ Tecnologías y Técnicas Utilizadas
Lenguaje: Python

Librerías: pandas, numpy, scikit-learn, imbalanced-learn, matplotlib, seaborn

Técnicas: SMOTE, GridSearchCV, permutation importance, VIF

Métricas clave: matriz de confusión, recall, precisión, F1-score, classification report

🔁 Pipeline de Modelado
Carga y limpieza de datos

Análisis exploratorio y visualización

Balanceo de clases con SMOTE

Entrenamiento de modelos base:

Random Forest

Regresión Logística

KNN

Árbol de Decisión

Ajuste de hiperparámetros con GridSearchCV

Evaluación con métricas orientadas a negocio

Interpretación de variables con permutation importance y VIF

Automatización del flujo para reproducibilidad

📈 Resultados y Comparación de Modelos

Modelo  ---   	Recall (Clase 1)---	 Precisión (Clase 1)---	 F1-score---	      Comentario
Random Forest	          0.82               	0.65	             0.73	          Buen balance entre recall y precisión
Regresión Logística	    0.76	              0.70	             0.73	          Más interpretable, pero menor recall
KNN	                    0.68	              0.60	             0.64	          Sensible al escalado y ruido
Árbol de Decisión	      0.74	              0.62	             0.67	          Fácil de visualizar, pero menos robusto

Nota: los valores son ilustrativos. Se deben actualizar con los resultados reales del proyecto.

📌 Conclusiones
El modelo con mejor desempeño en recall fue Random Forest, ideal para minimizar falsos negativos.

La interpretación de variables clave permite orientar campañas de retención más efectivas.

Se automatizó el pipeline para facilitar futuras iteraciones y pruebas con nuevos datos.

📎 Próximos Pasos
Validación cruzada con datos recientes

Pruebas en entorno productivo

Integración con sistemas de toma de decisiones comerciales
