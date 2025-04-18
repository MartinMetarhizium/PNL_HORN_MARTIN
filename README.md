#  Proyectos NLP

Este repositorio contiene una serie de notebooks desarrollados por **Martín Horn** como parte del proceso de aprendizaje en modelado de lenguaje y procesamiento de lenguaje natural (PLN), utilizando redes neuronales recurrentes (RNN) y LSTM. Se abordaron diferentes desafíos, progresivamente más complejos, enfocados en la generación de texto a nivel de caracteres, usando datasets reales como letras de canciones, diálogos de los libros de Harry Potter y embeddings de fasttext.

---

## 📁 Contenido

### 📘 `Desafio_1_Horn_Martin.ipynb`
**Objetivo:** Entrenamiento de un modelo LSTM para generación de texto a nivel de palabras, usando letras de canciones.

- Tokenización por palabras
- Padding manual con `Keras`
- Métrica de **perplejidad**
- Callback con early stopping
- Predicción secuencial simple (`generate_seq`)

---

### 📘 `Entregable_2_Horn_Martín.ipynb`
**Objetivo:** Reentrenamiento completo usando **tokenización a nivel de caracteres**, tal como fue solicitado por el docente.

- Uso del dataset de letras de canciones (`scrapped-lyrics-from-6-genres`)
- Tokenización a nivel de carácter
- Cambio del criterio de secuencias
- Mejora en la arquitectura LSTM
- Modelo más generalizable para generación letra por letra

---

### 📘 `Entregable_3_Horn_Martin.ipynb`
**Objetivo:** Cambiar el corpus de entrenamiento a un dominio más cerrado y temático: **diálogos de Harry Potter**.

- Dataset de Kaggle: `Harry Potter Dataset` (libros 1, 2 y 3)
- Limpieza y unión de archivos
- Tokenización por carácter
- Optimización del modelo:
  - Embedding de 128 dimensiones
  - LSTM con 256 unidades y dropout
  - `batch_size=128` y optimizador `Adam`
- Visualización de:
  - Cross-entropy
  - Perplejidad por época
- Gradio para generación interactiva
- Implementación de **beam search** para mejorar la calidad del texto generado

---

### 🤖 `Bot_Horn_Martin.ipynb`
**Objetivo:** Crear una interfaz interactiva con Gradio que permita generar texto a partir de una semilla, simulando una respuesta automática estilo chatbot.

- Entrenamiento del modelo en corpus reducido
- Uso de `Gradio` para desplegar un modelo generador interactivo
- Aplicación del modelo en tareas prácticas de NLP como:
  - autocompletado
  - generación creativa de texto
  - simulación de personaje

---

## 🚀 Principales aprendizajes

- Transición exitosa de modelado por palabras a modelado por caracteres
- Uso de métricas de evaluación propias del lenguaje como la **perplejidad**
- Entrenamiento y depuración de modelos LSTM recurrentes
- Optimización del rendimiento mediante arquitectura y datos
- Interactividad con interfaces modernas (`Gradio`)
- Exploración de estrategias de búsqueda como **beam search**

---

## 📚 Tecnologías utilizadas

- Python 3.10
- TensorFlow / Keras
- Pandas / NumPy
- Matplotlib / Seaborn
- Gradio
- KaggleHub
- Jupyter Notebook

---

## 📌 Requisitos

```bash
pip install tensorflow gradio pandas matplotlib kagglehub
```

---

## ✍️ Autor

**Martín Horn**  
Estudiante de Inteligencia Artificial Embebida – UBA  

