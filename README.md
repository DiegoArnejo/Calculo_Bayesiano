# Proyectos de Clasificación de Textos con Machine Learning

Este repositorio contiene dos proyectos desarrollados con Python para clasificar textos utilizando el algoritmo de **Naive Bayes** (`MultinomialNB`) y la vectorización de palabras (`CountVectorizer`).

---

## 📂 Contenido del Repositorio

### 1. Detector de Noticias Falsas 
* **Archivo:** `Bayes_Noticias.py` 
* **Objetivo:** Clasificar titulares automáticamente determinando si son **reales** o **falsos**.
* **Funcionamiento:** 
  1. Toma un conjunto de noticias etiquetadas previamente.
  2. Convierte las palabras en frecuencias numéricas con `CountVectorizer`.
  3. Entrena un modelo Naive Bayes con el 70% de los datos y evalúa su efectividad con el 30% restante.
  4. Permite evaluar nuevas noticias de prueba.

---

### 2. Detector de Mensajes de Grooming
* **Archivo:** `Bayes_Grooming.py`
* **Objetivo:** Detectar patrones de riesgo en conversaciones de chat para identificar situaciones de **grooming** frente a interacciones cotidianas o seguras (`no grooming`).
* **Funcionamiento:**
  1. Analiza frases y mensajes típicos de internet mediante procesamiento de texto.
  2. Emplea el mismo modelo probabilístico para identificar términos de alerta en los mensajes analizados.
  3. Evalúa el rendimiento del sistema mediante métricas de precisión y matriz de confusión.

---

## 🛠️ Tecnologías y Librerías Utilizadas
* **Python**
* **Pandas** (para el manejo de los datos y tablas)
* **Scikit-Learn (`sklearn`)**:
  * `CountVectorizer` (para transformar texto en datos numéricos)
  * `MultinomialNB` (algoritmo de clasificación Naive Bayes)
  * `train_test_split` (para dividir datos de entrenamiento y prueba)
  * `accuracy_score`, `classification_report`, `confusion_matrix` (para evaluar el rendimiento)
