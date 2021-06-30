---
description: >-
  Apuntes por capítulo del libro "Python Machine Learning: Machine Learning and
  Deep Learning with Python, scikit-learn, and TensorFlow 2, 3rd Edition"
---

# Machine Learning and Deep Learning with Python \(Libro\)

## Chapter 1: Giving Computers the Ability to Learn from Data

### Aprendizaje Supervisado <a id="Aprendizaje-Supervisado"></a>

Sabemos la respuesta correcta antes de entrenar al modelo.

#### **Clasificación**

Determina la posición de las entradas sabiendo los distintos grupos discretos de información. Por ejemplo:

* Esto es SPAM o no? \(clasificación binaria\)
* La letra que has escrito es una A, una B, una C, etc. \(clasificación multiclase\)

#### **Análisis de regresión**

Busca la función de regresión más cercana a los puntos \(normalmente con la media del cuadrado de la distancia a la recta\). Por ejemplo:

* Sabiendo que hay una relación entre el tiempo de estudio de un examen y su calificación final en el test, se puede elaborar un modelo que prediga la nota de un futuro alumno sabiendo el tiempo de estudio

#### **Aprendizaje por esfuerzo \(reinforcement learning\)**

El objetivo es desarrollar un agente que mejore sus respuestas recibiendo una señal de recompensa \(victoria/perdida\) del entorno \(reward signal\). Esta señal puede ser inmediata o aplazada, y el agente trata de maximizar la recompensa. Por ejemplo:

* Ajedrez: tu movimiento recibe una victoria si quitas una ficha del oponente o una pérdida si tu oponente retira una de tus fichas.

### Aprendizaje NO Supervisado

Intenta extraer la información relevante sin saber la función de recompensa o una variable resultado. El agente es quien tiene que “sacar la formula” sin saber la estructura de las variables.

#### **Clustering \(Clasificación no supervisada\)**

Es una clasificación en la que no tenemos información sobre los grupos \(solo se sabe cuántos grupos hay\). Por ejemplo:

* Preparación de campañas de marketing con el top 10 de intereses de los potenciales cliente.

#### **Reducción de dimensionalidad**

Se trata de eliminar el ruido del dataset y quedarnos con la información más relevante. Así, nuestro modelo no se entrenará con ruido y el dataset será más pequeño. Por ejemplo:

* Reduce una gráfica de 3D a 2D ignorando la dimensión que menos varía y, por tanto, menos relevancia tiene.

