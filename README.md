# README - Descripción de Datos y codigos

---
# Para Random Forest
este codigo se encuentra en metodos/RandomForest/RandomForest.ipynb

## 1. **train_data.csv**
Este archivo se encuentra en la carpeta dataset/RandomForest/train_data.csv

Este archivo contiene los datos utilizados para entrenar el modelo de clasificación del clima. Incluye variables meteorológicas y su respectiva etiqueta de clase.

### **Contenido:**

* **precipitation**: Cantidad de precipitación registrada.
* **temp_max**: Temperatura máxima diaria.
* **temp_min**: Temperatura mínima diaria.
* **wind**: Velocidad del viento.
* **weather**: Variable objetivo que representa la categoría del clima (0, 1, 2, 3 o 4).

### **Cómo se generó:**

* Los datos provienen de un conjunto original de observaciones meteorológicas.
* Se procesaron limpiando valores faltantes y corrigiendo inconsistencias.
* La etiqueta *weather* fue asignada de acuerdo con condiciones basadas en umbrales climáticos o clasificación previa.
* Este archivo se utiliza exclusivamente para el entrenamiento del modelo.

---

## 2. **test_data.csv**
Este archivo se encuentra en la carpeta dataset/RandomForest/test_data.csv

Archivo destinado a evaluar el desempeño del modelo entrenado.

### **Contenido:**

Posee las mismas columnas que *train_data.csv*:

* **precipitation**
* **temp_max**
* **temp_min**
* **wind**
* **weather**

### **Cómo se generó:**

* Se separó del dataset original siguiendo un proceso de selección aleatoria o cronológica (según diseño experimental).
* No se utiliza para entrenamiento, únicamente para evaluar métricas como precisión, recall, f1-score y matriz de confusión.

---

# Para Gradient Boosting 
este codigo se encuentra en metodos/GradientBoosting/GradientBoosting.ipynb

## 1. **seattle-weather.csv**
Este archivo se encuentra en la carpeta dataset/GradientBoosting

### **Contenido:**

* **date**
* **todos los demas de Random Forest**

Este archivo es igual al de train_data.csv, pero no fue separado en test_data.csv. En el codigo del metodo Gradient se encarca de separar el archivo en train y test

---

