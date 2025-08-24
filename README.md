
# 🌳 Proyecto: Árbol de Decisión estilo RapidMiner (pero con Python 🐍 en Google Colab)

## 📌 Introducción

El objetivo principal de este proyecto es aplicar un **Árbol de Decisión** para predecir el **estado civil** de una persona a partir de características como:

* `casa` 🏠
* `guapo` 😎
* `edad` 🎂
* `dinero` 💵
* `estado_civil` ❤️

En un inicio, la tarea estaba pensada para realizarse en **RapidMiner**, pero debido a un pequeño incidente tecnológico ⚡💻 (mi computadora hizo corto y tuve que trabajar en una laptop prestada ), decidí **buscar la equivalencia en Python** usando **Google Colab**.

Spoiler: el resultado fue incluso más potente y profesional.

---

## 🔄 Equivalencia con lo que pedía en RapidMiner

| RapidMiner 🛠️         | Python / Colab 🐍                                                                             |
| ---------------------- | --------------------------------------------------------------------------------------------- |
| Ingesta de datos       | `pandas.read_excel()` o `pandas.read_csv()`                                                   |
| Manipulación básica    | Métodos de `pandas`: `head()`, `info()`, `describe()`, limpieza de nulos, conversión de tipos |
| Modelo de Árbol        | `DecisionTreeClassifier` de `scikit-learn`                                                    |
| Interpretación gráfica | `plot_tree` (básico) + `Graphviz` (visualización profesional)                                 |

---

## ⚙️ Pasos desarrollados

1. **Ingesta de datos** 📥

   * Se cargó el dataset `soltero.xlsx` con `pandas`.
   * Se revisaron tipos de datos, valores nulos y estadísticas descriptivas.

2. **Aplicación del modelo de ML** 🤖

   * Se entrenó un árbol de decisión usando `scikit-learn`.
   * Se utilizó el criterio `entropy` (ganancia de información) para acercarnos a la lógica de RapidMiner.

3. **Visualización del Árbol** 🌳

   * Inicialmente con `plot_tree` de `matplotlib`.
   * Finalmente mejorado con **Graphviz**, que ofrece un diseño más claro, con colores y nodos redondeados.

4. **Interpretación y presentación** 🎯

   * Se evaluó la importancia de las variables (`feature_importances_`).
   * Se identificaron reglas clave (ejemplo: dinero y edad como principales predictores).
   * Se armó una presentación ejecutiva en 5 slides con objetivos, desarrollo, gráfica y conclusiones.

---

## 😂 Nota personal

> Sí, la idea era hacerlo en RapidMiner… pero la computadora decidió hacer un **“plot twist” eléctrico** ⚡ y terminé en Colab, con una laptop prestada.
>
> Resultado: aprendí que **cuando la vida te quita RapidMiner, ¡tú instalas pandas y scikit-learn!** 🐼🤓

---

## 📊 Conclusiones

* Python no solo reemplazó a RapidMiner, sino que permitió un mayor control del flujo.
* La visualización con **Graphviz** ofrece un resultado más profesional para informes.
* Este ejercicio es una muestra de cómo trasladar flujos de **low-code (RapidMiner)** a **full-code (Python)** sin perder claridad.

---

## 🚀 Cómo ejecutar

1. Sube el archivo `soltero.xlsx` a tu Google Colab.
2. Copia el notebook y ejecuta las celdas.
3. Genera tu árbol de decisión y descárgalo en PNG para tus presentaciones.


