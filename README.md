# Desafios practicos (curso de PLN)

Este repositorio contiene el desarrollo de los **cuatro desafíos prácticos** de la asignatura **Procesamiento del Lenguaje Natural (PLN)**, realizados por **Jorge Vásquez**.  

---

## 📂 Estructura del repositorio

El repositorio está organizado en cuatro carpetas principales, con una notebook por cada desafío.
Cada notebook contiene el código, resultados, análisis y conclusiones correspondientes a su desafío.

---

## Desafío 1 — Vectorización y Clasificación de Documentos

**Objetivo:** Analizar la representación vectorial de documentos y su uso en tareas de similaridad y clasificación.

**Actividades realizadas:**
1. **Vectorización de documentos:** Selección de 5 documentos al azar y cálculo de similaridad con el resto para analizar coherencia semántica.
2. **Clasificación por prototipos (Zero-Shot):** Asignación de clases a documentos de test basándose en la similaridad con los de entrenamiento.
3. **Modelos de Naïve Bayes:** Entrenamiento y ajuste de modelos *MultinomialNB* y *ComplementNB* para maximizar el *F1-score macro*.
4. **Vectorización de palabras:** Transposición de la matriz documento-término para estudiar la similaridad entre palabras seleccionadas.

---

## Desafío 2 — Embeddings de Palabras con Gensim

**Objetivo:** Crear representaciones vectoriales (embeddings) propias a partir de corpus textuales.

**Actividades realizadas:**
1. Entrenamiento de **modelos Word2Vec** con **Gensim**, utilizando letras de canciones como corpus.
2. Exploración de términos de interés y análisis de similitud semántica entre palabras.
3. Visualización de los embeddings en el espacio vectorial.
4. Confirmar que los embeddings entrenados con Gensim reflejan el contexto específico en el que cada palabra aparece en las canciones, diferente al sentido general que tendrían en otro corpus (ej. noticias, Wikipedia).

---

## Desafío 3 — Modelos de lenguaje y generación de secuencias.

**Objetivo:** Implementar un **modelo de lenguaje con tokenización por caracteres,** basado en redes neuronales recurrentes (RNN, LSTM, GRU).

**Actividades realizadas:**
1. Selección y **preprocesamiento de un corpus** de texto para tokenización por caracteres.
2. Creación del dataset y división en entrenamiento y validación.
3. Implementación de modelos basados en **SimpleRNN**, **LSTM** y **GRU**, entrenados con *rmsprop*.
4. Generación de texto utilizando estrategias de:
   - **Greedy Search**
   - **Beam Search** (determinístico y estocástico)
5. Análisis del efecto de la **temperatura** en la generación de texto con beam estocastico.

---

## Desafío 4 — Traductor con LSTM (modelos Seq2Seq)

**Objetivo:** Implementar un **modelo traductor de inglés a español** basado en redes LSTM con arquitectura **encoder–decoder**.

**Actividades realizadas:**
1. **Replicar y mejorar** un modelo de traducción de inglés a español seq2seq (encoder-decoder) utilizando **PyTorch**.
2. Entrenamiento extendido con más datos y secuencias más largas.
3. Estudio del impacto del número de neuronas en las capas recurrentes.
4. Presentación de **5 ejemplos de traducciones generadas**.
5. (Opcional) Experimentos con **embeddings preentrenados** (Glove/FastText) y estrategias de generación alternativas (como muestreo aleatorio).

---
