# 🍌🍅 YOLO 11 - Detección de Frutas Frescas y Podridas

Este proyecto implementa un modelo de detección de objetos utilizando **YOLO v11** para identificar el estado de frutas comunes como **tomate**, **banana** y **naranja**. El modelo es capaz de diferenciar entre frutas **frescas** y **podridas**, siendo útil para tareas de clasificación, control de calidad, y aplicaciones agrícolas automatizadas.

---

## 📁 Dataset

El dataset fue creado y anotado utilizando la plataforma [Roboflow](https://roboflow.com/), incluyendo imágenes de:

- **Tomates**
  - Tomate fresco
  - Tomate podrido
- **Bananas**
  - Banana fresca
  - Banana podrida
- **Naranjas**
  - Naranja fresca
  - Naranja podrida

También se incluyeron **imágenes negativas** (sin frutas o con otros objetos) como contraejemplos para mejorar la precisión del modelo y reducir falsos positivos.

---

## 🧪 División del Dataset

El dataset fue exportado desde Roboflow en formato YOLO y luego dividido en Python utilizando scripts personalizados para garantizar una correcta proporción de datos:

- `train/`: 70%
- `val/`: 20%
- `test/`: 10%

---

## ⚙️ Tecnología usada

- **YOLO v11** (You Only Look Once, versión 11)
- **Python**
- **CUDA** para aceleración en GPU
- **Visual Studio** (para compilación y pruebas en tiempo real)
- **Roboflow** (anotación y preprocesamiento del dataset)

---

## 🧠 Entrenamiento del modelo

- Se entrenó el modelo con imágenes etiquetadas desde Roboflow.
- Se ajustaron hiperparámetros para mejorar la precisión.
- Se utilizó detección en tiempo real mediante cámara con CUDA activado.
- Se monitorearon métricas como `mAP`, `Precision`, `Recall` durante el entrenamiento.

---

## 🖼️ Ejemplos de detección

El modelo puede identificar múltiples frutas en una sola imagen y distinguir entre sus estados. Aquí algunos ejemplos:

- ✅ Tomate fresco detectado correctamente.
- ⚠️ Banana podrida identificada en condiciones de poca luz.
- ❌ Imagen vacía correctamente ignorada como negativa.

---
## 🧑‍💻 Autor

**Marck0820001**  
Repositorio: [Model-of-ML-using-Yolo-for-fruit-deteccion](https://github.com/marck0820001/Model-of-ML-using-Yolo-for-fruit-deteccion)
