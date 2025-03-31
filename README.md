# 🧠 Predicción de Ingresos con el Dataset Adult (Census Income)

Este proyecto utiliza algoritmos de Machine Learning para predecir si una persona gana más de 50K al año, basándose en información socioeconómica del censo de EE.UU. de 1994.

---

## 📊 Dataset

- **Nombre**: Adult / Census Income
- **Fuente**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/adult)
- **Registros**: ~48,000
- **Objetivo**: `income` → `>50K` o `<=50K`

---

## ⚙️ Tecnologías y librerías usadas

- Python 3
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## 🚀 Cómo usar

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/babuenop/machine-learning-basics.git
   cd machine-learning-basics
   ```

2. Instalar dependencias:
   ```bash
   pip install -r requirements.txt
   ```

3. Ejecutar el notebook:
   - `03_ProyectoFinal.ipynb`


---

## 📂 Contenido del proyecto

- Limpieza y preprocesamiento de datos
- Entrenamiento de dos modelos:
  - Regresión Logística
  - Random Forest
- Evaluación con métricas:
  - Precisión, Recall, F1-score, Accuracy
- Matriz de confusión visual
- Interpretación de importancia de variables
- Predicción de nuevos casos

---

## 🧪 Ejemplo de predicción

Dado un nuevo caso como este:

```python
{'age': 52, 'education': 'Masters', 'hours_per_week': 55, ...}
```

El modelo Random Forest predice: `>50K`

---

## 📈 Importancia de variables (Random Forest)

Las variables con mayor influencia en la predicción fueron:
- `education_num`
- `capital_gain`
- `hours_per_week`
- `age`
- `marital_status_Married-civ-spouse`

---

## 🧠 Conclusión

- Ambos modelos lograron una **exactitud superior al 85%**
- **Random Forest** tuvo mejor rendimiento general:
  - Accuracy: 85.69%
  - Mejor equilibrio entre clases
  - Más robusto sin necesidad de escalar
- **Regresión Logística** es útil por su interpretabilidad, pero fue superada en desempeño

✅ *Random Forest es el modelo recomendado para este problema.*

---

## 📌 Autor
Proyecto personal de aprendizaje en Machine Learning con Python y datos reales.

---

## 📦 Requisitos

Contenido sugerido para `requirements.txt`:

```
pandas
numpy
scikit-learn
matplotlib
```

Generalo automáticamente con:

```bash
pip freeze > requirements.txt
```