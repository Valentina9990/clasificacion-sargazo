# 🌿 Clasificación de Sargazo en el Caribe Mexicano

## 📘 Descripción del problema
El Caribe Mexicano se ha visto gravemente afectado por el arribo masivo de **sargazo** en los últimos años.  
Este proyecto busca **estimar la cantidad de sargazo** presente en las playas mediante el **análisis automático de imágenes**.

El objetivo principal es construir un modelo de **clasificación de imágenes** que, dada una fotografía de una playa, determine el **nivel de sargazo** presente.

---

## 🧠 Objetivo
Desarrollar un modelo de **aprendizaje automático (machine learning)** o **aprendizaje profundo (deep learning)** capaz de clasificar imágenes en distintos niveles de presencia de sargazo.

---

## 🗂️ Conjunto de datos
El conjunto de datos fue creado recopilando imágenes de publicaciones públicas en **Facebook** e **Instagram**.  
Estas imágenes fueron **almacenadas localmente y etiquetadas manualmente**.

### 📑 Estructura de las etiquetas
Cada imagen tiene asociadas cuatro etiquetas:

| Etiqueta | Descripción |
|-----------|-------------|
| **lugar** | Playa o zona donde fue tomada la imagen |
| **fecha** | Fecha de captura de la imagen |
| **nivel** | Cantidad de sargazo presente |
| **escena** | Tipo de escena (por ejemplo, orilla, mar abierto, playa completa, etc.) |

### 🌊 Niveles de sargazo
La etiqueta **nivel** indica la cantidad de sargazo observada en la imagen.  
Los niveles están definidos en español y siguen un orden incremental:

| Nivel (ES) | Nivel (EN) | Descripción |
|-------------|-------------|-------------|
| `nada` | none | Sin presencia de sargazo |
| `bajo` | low | Presencia leve |
| `moderado` | mild | Presencia moderada |
| `abundante` | plenty | Alta concentración |
| `excesivo` | excessive | Cobertura total o casi total |

> ⚠️ El conjunto de datos es **desequilibrado**, con mayor cantidad de ejemplos en los niveles "nada" y "bajo".

---

## 💻 Solución propuesta
Se permite utilizar **cualquier enfoque de aprendizaje automático** para resolver el problema.  
Como referencia, se provee un ejemplo utilizando **redes neuronales convolucionales (CNN)** con arquitecturas preentrenadas como:

- ResNet  
- VGG  
- GoogleNet  
- InceptionV3  

Estas redes pueden ser ajustadas (fine-tuning) para la clasificación de imágenes del dataset de sargazo.

---

## 🚀 Instrucciones de uso

### 1️⃣ Descarga del conjunto de datos
Puedes obtener los datos directamente desde **Kaggle** usando el siguiente comando:

```bash
kaggle competitions download -c meia-2025-sargazo-prediction
