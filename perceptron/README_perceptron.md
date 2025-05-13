
# 🧠 Perceptrón: Fundamentos, Matemática y Visualización

Este proyecto explica desde cero el concepto del **Perceptrón**, uno de los modelos fundamentales en el campo de la inteligencia artificial y aprendizaje automático. Está inspirado en el libro _"Neural Networks and Deep Learning"_ de Charu C. Aggarwal, y pensado para estudiantes que deseen **entender, programar y visualizar** el algoritmo de manera didáctica.

---

## 🔎 ¿Qué es un Perceptrón?

El **perceptrón** es el modelo más simple de una neurona artificial. Fue propuesto por Frank Rosenblatt en 1958 y sirve como clasificador binario lineal. Dado un conjunto de entradas numéricas (features), el perceptrón intenta aprender un **hiperplano de separación** que divida correctamente dos clases distintas.

---

## 📐 Ecuación del modelo

El perceptrón toma una entrada `x` (un vector de características) y predice una etiqueta mediante la función de activación **signo** (`sign`):

```math
\hat{y} = \text{sign}( \mathbf{w}^\top \mathbf{x} + b )
```

📖 **Lectura matemática precisa**:  
“La y sombrero es igual al signo de el producto punto entre el vector de pesos w transpuesto y el vector de características x, más el sesgo b.”

---

## 🎯 Objetivo de entrenamiento

El objetivo del perceptrón es encontrar los pesos `w` y el sesgo `b` que clasifiquen correctamente todos los ejemplos de entrenamiento linealmente separables.  
Se usa una regla de aprendizaje muy simple basada en errores:

- Si una predicción es incorrecta, se **actualizan** los pesos y el sesgo:
  
```math
\mathbf{w} \leftarrow \mathbf{w} + \eta \cdot y_i \cdot \mathbf{x}_i
```
```math
b \leftarrow b + \eta \cdot y_i
```

📖 **Lectura**:  
“w se actualiza como w más el producto de eta por y sub i por x sub i.  
b se actualiza como b más eta por y sub i.”

---

## ⚙️ Implementación en Python

El código incluido en este repositorio:

- Genera un conjunto de datos 2D simple con dos clases linealmente separables.
- Implementa el algoritmo de entrenamiento del perceptrón desde cero.
- Visualiza el conjunto de datos, la frontera de decisión y el comportamiento del modelo.

📁 Estructura de archivos:

```
📦 perceptron
 ┣ 📜 perceptron.py        # Implementación principal
 ┣ 📜 README.md            # Este archivo
 ┗ 📊 gráfica.png          # Visualización del resultado
```

---

## 📊 Visualización

La visualización muestra:

- Puntos de datos con colores por clase.
- Frontera de decisión aprendida.
- Cambios de la línea separadora a lo largo de las épocas (si se activa animación).

Este enfoque visual ayuda a **entender intuitivamente** cómo el perceptrón ajusta los pesos para encontrar una solución.

---

## ⚠️ Limitaciones del Perceptrón

- Solo funciona correctamente si los datos son **linealmente separables**.
- No aprende probabilidades, solo clases (+1 o -1).
- No converge si los datos son ruidosos o no separables linealmente.

---

## 🧠 ¿Qué aprendés con este proyecto?

- Fundamentos de redes neuronales.
- Implementación desde cero de un modelo de IA.
- Cómo se entrena una red con errores.
- El rol de los vectores de características y pesos.
- Visualización de modelos en 2D.

---

## 🗂️ Requisitos

- Python 3.7+
- numpy
- matplotlib

Instalación:

```bash
pip install numpy matplotlib
```

---

## 🎥 Video explicativo

👉 Pronto disponible en YouTube  
📎 [Enlace al repositorio y ejemplo visual]()

---

## 📚 Referencias

- Charu C. Aggarwal — *Neural Networks and Deep Learning*
- F. Rosenblatt (1958) — *The Perceptron: A Probabilistic Model for Information Storage and Organization in the Brain*
- [Wikipedia: Perceptron](https://es.wikipedia.org/wiki/Perceptr%C3%B3n)

---

## 🤖 Autor

Tony Gael — Estudiante de Licenciatura en Inteligencia Artificial y Robótica  
Contribuciones educativas con fines didácticos.
