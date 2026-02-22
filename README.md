# NLP Práctica – Reseñas Musicales
## 📌 Descripción
Este proyecto implementa un flujo completo de Procesamiento de Lenguaje Natural (NLP) sobre reseñas de productos musicales. El objetivo es explorar, limpiar y modelar el texto para predecir el sentimiento asociado a las reseñas, utilizando el rating (overall) como etiqueta de clasificación.
## 📂 Estructura del repositorio
```text
├── data/        # Dataset original y versiones procesadas
├── notebooks/   # Exploración, preprocesamiento, modelado y conclusiones
├── scripts/     # Funciones auxiliares y módulos reutilizables
└── README.md    # Descripción del proyecto


## 🔎 Exploración de datos
- Distribución de ratings (overall).
- Longitud promedio de reseñas.
- Cardinalidad del vocabulario.
- Wordclouds comparativos (reseñas positivas vs negativas).
- N-grams más frecuentes.
## 🛠️ Preprocesamiento
- Selección de columnas relevantes (reviewText, overall).
- Limpieza básica inicial con RegEx y split().
- Pipeline híbrido de limpieza:
- Tokenización con NLTK.
- Lematización con SpaCy.
- Eliminación de stopwords y normalización de texto.
- Codificación de etiquetas (positivo/negativo).
## 🤖 Modelado
- Representación vectorial con TF-IDF.
- Entrenamiento de modelos de clasificación supervisada.
- Aplicación de undersampling para balancear las clases y evitar sesgos.
- Implementación de un modelo de Deep Learning estilo IMDB:
- Secuencias de texto convertidas en índices.
- Capa de Embedding para representar palabras.
- Arquitectura con LSTM para capturar dependencias temporales en el texto.
- Evaluación con métricas: accuracy, F1-score, matriz de confusión.
## 📊 Resultados
- Comparación de desempeño entre modelos con datos crudos vs datos limpiados.
- Evidencia de mejora al aplicar el pipeline híbrido de limpieza.
- Resultados del modelo LSTM frente a enfoques clásicos (TF-IDF / regresión logística).
- Conclusiones sobre vocabulario y patrones de reseñas.
- Documentación incluida en los notebooks.
## 🚀 Reproducibilidad
- Clonar el repositorio:
git clone https://github.com/Fablop84/NLP_entrega_practica.git
- Instalar dependencias:
pip install -r requirements.txt
- Ejecutar notebooks en notebooks/ para reproducir análisis y entrenamiento.


