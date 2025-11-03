# A3.2 Redes Neuronales

Este proyecto utiliza redes neuronales para clasificar imágenes de dígitos del 0 al 9, empleando la base de datos **MNIST** y un conjunto adicional de imágenes personalizadas.  
El objetivo es entrenar un modelo capaz de reconocer dígitos escritos a mano, evaluar su desempeño en distintos conjuntos de datos y explorar mejoras que optimicen su precisión y funcionalidad.

---

## Datos utilizados

- **Imágenes del conjunto MNIST**: 28×28 píxeles en escala de grises.  
- **Etiquetas del 0 al 9** que indican el dígito representado.  
- **Imágenes personalizadas** generadas por el usuario para evaluar el modelo en condiciones reales.  
- Las imágenes adicionales fueron preprocesadas para adaptarse al formato esperado por el modelo.

---

## Metodología

### 1. Entrenamiento del modelo
- Se construyó una red neuronal utilizando TensorFlow/Keras.
- Se entrenó el modelo con el conjunto MNIST, aplicando técnicas como *early stopping* para evitar sobreajuste.
- Se graficó la evolución de la precisión y la pérdida durante el entrenamiento.

### 2. Evaluación en conjunto de prueba
- Se calculó la exactitud del modelo sobre el conjunto de prueba de MNIST.
- Se comparó con la exactitud obtenida en validación para analizar el comportamiento del modelo.

### 3. Prueba con imágenes personalizadas
- Se generaron imágenes nuevas, 5 por cada dígito.
- Se aplicó un preprocesamiento para adaptar las imágenes al formato MNIST.
- Se evaluó el modelo sobre estas imágenes y se compararon los resultados con los obtenidos en entrenamiento y prueba.

### 4. Análisis de errores
- Se identificaron casos en los que el modelo falló.
- Se discutieron posibles causas como diferencias de formato, ruido, iluminación o trazos irregulares.

### 5. Mejoras al sistema
- Se implementaron tres mejoras en distintas etapas del flujo:
  - Ajustes en el preprocesamiento para mejorar la calidad visual.
  - Visualización detallada de resultados por imagen.
  - Evaluación de exactitud con métricas adicionales.
- Se analizó si estas mejoras impactaron positivamente en la precisión o funcionalidad.

### 6. Predicción en tiempo real
- Se desarrolló un sistema que utiliza la cámara de la computadora para capturar imágenes.
- Se preprocesa cada cuadro en tiempo real y se realiza la predicción del dígito mostrado.
- Se muestra en pantalla la clase predicha junto con la imagen procesada.

---

## Archivos del proyecto

- [Reporte en ipynb](A3_2_648241.ipynb)  
- [Reporte en html](A3_2_648241.html)  
- [Modelo](user_images.zip)  
- [Sistema en tiempo real](realtime_digit_detection.py)
