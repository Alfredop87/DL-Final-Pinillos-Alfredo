# Predictive Maintenance with Deep Learning for Operational Failure Prediction

## 📌 Descripción del Proyecto

Las fallas operativas en equipos industriales pueden generar paradas no programadas, pérdidas económicas y riesgos para la seguridad. En este contexto, el mantenimiento predictivo permite anticipar estas fallas mediante el análisis de datos operativos.

El objetivo de este proyecto es desarrollar un modelo de deep learning capaz de predecir fallas en equipos industriales a partir de variables de operación, contribuyendo a mejorar la confiabilidad operativa y la toma de decisiones.

---

## 🎯 Objetivo

Construir y evaluar un modelo de red neuronal (MLP) para predecir fallas operativas utilizando el dataset **AI4I 2020 Predictive Maintenance**.

---

## 📊 Dataset

Se utiliza el dataset:

**AI4I 2020 Predictive Maintenance Dataset**

Contiene variables como:

- Tipo de máquina  
- Temperatura del aire  
- Temperatura del proceso  
- Velocidad de rotación  
- Torque  
- Desgaste de herramienta  

Variable objetivo:

- `Machine failure` (0 = No falla, 1 = Falla)

⚠️ Nota: No se sube el dataset al repositorio. Se carga directamente desde una fuente pública.

---

## ⚙️ Metodología

El proyecto sigue los siguientes pasos:

1. Exploración de datos (EDA)
2. Preprocesamiento:
   - Eliminación de variables irrelevantes
   - Codificación de variables categóricas
   - Escalamiento de variables
3. División en entrenamiento y prueba
4. Implementación de modelos:
   - Modelo baseline: Regresión Logística
   - Modelo principal: Red Neuronal (MLP)
5. Evaluación con métricas:
   - Accuracy
   - Precision
   - Recall
   - F1-score

---

## 🤖 Modelos Implementados

### 🔹 Modelo Baseline
Regresión Logística utilizada como referencia para evaluar el desempeño del modelo de deep learning.

### 🔹 Modelo Deep Learning
Red neuronal con la siguiente arquitectura:

- Capa densa (32 neuronas, ReLU)
- Dropout
- Capa densa (16 neuronas, ReLU)
- Dropout
- Capa de salida (sigmoid)

---

## 📈 Resultados

Ejemplo de métricas obtenidas:

| Modelo | Accuracy | Recall | F1-score |
|--------|--------|--------|---------|
| Regresión Logística | 0.96 | 0.62 | 0.70 |
| Red Neuronal | 0.97 | 0.68 | 0.75 |

El modelo de red neuronal muestra una mejora en la capacidad de capturar relaciones no lineales en los datos.

---

## 🧠 Interpretación

Debido al desbalance del dataset, la métrica más relevante es el **recall**, ya que permite evaluar la capacidad del modelo para detectar fallas reales.

No detectar una falla en un entorno industrial puede generar consecuencias críticas, por lo que minimizar falsos negativos es clave.

---

## 🏭 Aplicación en la Industria

Este modelo puede aplicarse en:

- mantenimiento predictivo
- gestión de activos industriales
- optimización de costos de mantenimiento
- mejora de confiabilidad operativa

En industrias como energía, manufactura y petróleo, este tipo de soluciones puede generar un impacto significativo en seguridad y eficiencia.

---

## ▶️ Ejecución del Proyecto

El notebook principal se encuentra en:

notebooks/final_project.ipynb

El proyecto puede ejecutarse directamente en **Google Colab**.

✔ El notebook es completamente reproducible  
✔ Se ejecuta de inicio a fin sin errores  

---

## 📹 Video Explicativo

Enlace al video (YouTube):

https://youtu.be/UlHYTV59iew

---

## 🧾 Estructura del Repositorio

DL-Final-Pinillos-Alfredo/
│
├── notebooks/
│ └── final_project.ipynb
│
├── README.md


---

## 🚀 Conclusiones

Se demostró que es posible predecir fallas operativas utilizando modelos de deep learning basados en datos de operación.

La red neuronal presenta un mejor desempeño frente al modelo baseline, evidenciando su capacidad para capturar patrones complejos.

Este enfoque puede ser extendido a aplicaciones reales de monitoreo y mantenimiento predictivo en entornos industriales.

---

## 📌 Mejoras Futuras

- Balanceo de clases  
- Optimización de hiperparámetros  
- Evaluación de modelos adicionales  
- Implementación en sistemas de monitoreo en tiempo real  
