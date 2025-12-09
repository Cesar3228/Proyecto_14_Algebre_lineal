# Proyecto_14_Algebre_lineal
## Machine Learning y protección de datos personales (Sure Tomorrow)  
## Machine Learning and Personal Data Protection (Sure Tomorrow)

---

## 🧩 Descripción general / Overview

### 🇪🇸 Español

La compañía de seguros **Sure Tomorrow** desea evaluar cómo el **Machine Learning** puede apoyar distintos problemas de negocio, al mismo tiempo que se protege la información personal de los clientes.

En este proyecto se abordan **cuatro tareas principales**:

1. Identificar clientes **similares** a un cliente dado para apoyar estrategias de marketing.
2. Predecir si un cliente es **probable beneficiario de seguros**, comparando un modelo entrenado con un modelo *dummy*.
3. Predecir la **cantidad de beneficios de seguro** que recibirá un cliente mediante un modelo de regresión lineal.
4. Implementar un método de **ofuscación de datos** que proteja la información personal sin afectar la calidad del modelo predictivo.

El proyecto demuestra cómo utilizar modelos de machine learning de forma responsable, manteniendo un equilibrio entre **utilidad del modelo y privacidad de los datos**.

Este proyecto corresponde al **Proyecto 14 – Machine Learning y privacidad de datos** del programa de **Data Science de TripleTen**.

---

### 🇬🇧 English

The insurance company **Sure Tomorrow** wants to evaluate how **Machine Learning** can support several business tasks while ensuring the protection of customers’ personal data.

This project addresses **four main tasks**:

1. Identifying customers **similar** to a given client to support marketing strategies.
2. Predicting whether a customer is **likely to receive insurance benefits**, comparing a trained model with a *dummy* model.
3. Predicting the **number of insurance benefits** a customer may receive using linear regression.
4. Implementing a **data obfuscation** method that protects personal information without degrading model performance.

The project demonstrates how machine learning models can be used responsibly, balancing **model usefulness and data privacy**.

This project corresponds to **Project 14 – Machine Learning and Data Privacy** in the **TripleTen Data Science program**.

---

## 📂 Datos / Data

### Dataset
- Archivo / File: `/datasets/insurance_us.csv`

### Características / Features
- `sex` — sexo de la persona asegurada  
- `age` — edad  
- `salary` — salario anual  
- `family_members` — número de familiares  

### Variable objetivo / Target
- `insurance_benefits` — número de beneficios de seguro recibidos en los últimos cinco años

> **Nota / Note:**  
> El dataset no se incluye en este repositorio debido a restricciones de la plataforma **TripleTen**.  
> The dataset is not included due to **TripleTen platform restrictions**.

---

## 🔍 Metodología / Methodology

### 🇪🇸 Español

1. **Carga y validación de datos**
   - Revisión de valores faltantes.
   - Identificación de valores atípicos.
   - Verificación de tipos de datos.

2. **Tarea 1: Búsqueda de clientes similares**
   - Uso de métricas de distancia para encontrar clientes con características cercanas.
   - Aplicación práctica en marketing personalizado.

3. **Tarea 2: Clasificación de beneficiarios**
   - Entrenamiento de un modelo de clasificación para predecir si un cliente recibirá beneficios.
   - Comparación contra un **modelo dummy**.
   - Análisis de cuándo un modelo entrenado puede ser mejor o peor que uno no entrenado.

4. **Tarea 3: Predicción del número de beneficios**
   - Construcción de un modelo de **regresión lineal**.
   - Evaluación del desempeño del modelo con métricas apropiadas.

5. **Tarea 4: Ofuscación de datos**
   - Desarrollo de un algoritmo de transformación de datos.
   - Protección de información personal sensible.
   - Verificación de que el modelo entrenado con datos ofuscados mantiene la misma calidad predictiva que el modelo original.

6. **Conclusiones**
   - Análisis de resultados.
   - Reflexión sobre el uso ético del machine learning y la protección de datos.

---

### 🇬🇧 English

1. **Data loading and validation**
   - Checking for missing values.
   - Identifying outliers.
   - Verifying data types.

2. **Task 1: Finding similar customers**
   - Using distance-based methods to identify similar customers.
   - Practical application for personalized marketing.

3. **Task 2: Benefit classification**
   - Training a classification model to predict whether a customer will receive benefits.
   - Comparison against a **dummy model**.
   - Analysis of when a trained model can outperform or underperform a dummy model.

4. **Task 3: Predicting benefit amounts**
   - Building a **linear regression** model.
   - Evaluating model performance using appropriate metrics.

5. **Task 4: Data obfuscation**
   - Implementing a data transformation algorithm.
   - Protecting sensitive personal information.
   - Verifying that model performance remains unchanged after data obfuscation.

6. **Conclusions**
   - Results analysis.
   - Discussion on ethical machine learning and data privacy.

---

## 🤖 Modelos utilizados / Models Used

- Algoritmos basados en distancia (similitud de clientes)
- Modelo de clasificación supervisada
- **Dummy classifier** como baseline
- **Regresión lineal**
- Modelo de regresión entrenado con datos ofuscados

---

## 📊 Resultados / Results

### 🇪🇸 Español

Los resultados muestran que:

- Los clientes similares pueden identificarse de manera efectiva a partir de características demográficas y económicas.
- Un modelo entrenado generalmente supera a un modelo *dummy*, aunque en escenarios con poco poder predictivo ambos pueden tener un desempeño similar.
- La regresión lineal permite estimar razonablemente el número esperado de beneficios de seguro.
- La ofuscación de datos protege la información personal sin degradar la calidad del modelo predictivo.

---

### 🇬🇧 English

The results show that:

- Similar customers can be effectively identified using demographic and economic features.
- A trained model generally outperforms a *dummy* model, although in low-signal scenarios their performance may be similar.
- Linear regression provides reasonable estimates of expected insurance benefits.
- Data obfuscation protects personal information without degrading predictive model performance.

---

## 📁 Estructura del repositorio / Repository Structure

```text
.
├── Proyecto_14.ipynb
├── requirements.txt
└── README.md
