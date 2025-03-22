# DSIII_PF-NLP-y-NN_Guardia
Entrega final correspondiente a la realizacion de 2 ejercicios una relativo a NLP y NN

## Ejercicio 1: Detección de Fake News (NLP)

Se desarrolló un modelo de procesamiento de lenguaje natural (NLP) para clasificar noticias como **reales o falsas**.  
- Se trabajó con un dataset balanceado de noticias en inglés **fake_or_real_news.csv**.
- Se aplicaron técnicas de preprocesamiento de texto: limpieza, tokenizacion, lematización, stopwords.
- Se entrenaron y compararon dos modelos:
  - **Multinomial Naive Bayes** (modelo probabilístico)
  - **Passive-Aggressive Classifier** (modelo absolutista)
- Se evaluaron métricas como **accuracy, precision, recall y f1-score**.
- Se concluyó que el modelo Passive-Aggressive tuvo mejor rendimiento para el objetivo del ejercicio.

El código se encuentra en el notebook: NLP_Entrega Final_Fake News_Guardia Maria Eugenia.

## Ejercicio 2: Clasificación de imágenes con Redes Neuronales (Fashion MNIST)

Se desarrolló un modelo de red neuronal para clasificar imágenes de prendas de vestir en **10 categorías**.  
- Se trabajó con el dataset **Fashion MNIST**, que contiene imágenes de 28x28 píxeles en escala de grises.
- Se entrenaron y compararon dos modelos secuenciales:
  - **Modelo Sencillo**: tres capas densas (512, 256 y 128 neuronas).
  - **Modelo Mejorado**: misma base que el modelo sencillo + dos capas adicionales (64 y 32 neuronas).
- Ambos modelos utilizaron ReLU como activación interna y softmax en la capa de salida.
- Se entrenaron durante 5 épocas usando adam como optimizador y sparse_categorical_crossentropy como función de pérdida.
- Se compararon métricas como **accuracy final, mejor val_accuracy y mejor val_loss**.
- Se concluyó que el modelo mejorado tuvo un rendimiento **ligeramente superior**, sin presentar señales de sobreajuste.

El código se encuentra en el notebook: NN_Entrega Final_Fashion MNIST_Maria Eugenia Guardia.
