# Proyectos de Clasificación de Imágenes y Nube de Palabras

---
## 1. Proyecto Nube de Palabras

### Descripción
Este proyecto genera una nube de palabras a partir de un corpus de texto, representando gráficamente la frecuencia de palabras mediante tamaños proporcionales. El proyecto se centra en analizar las palabras clave en un texto relacionado con las personas y los términos que las rodean, revelando así patrones de interacción y lenguaje.

### Bibliotecas Principales
- **Pandas**: Para la manipulación de datos.
- **Matplotlib & Seaborn**: Para la visualización de datos.
- **WordCloud**: Generación de la nube de palabras.
- **Natural Language Toolkit (nltk)**: Procesamiento del lenguaje natural, incluyendo eliminación de stopwords y stemming.

### Pasos Realizados:
1. **Limpieza del Texto**: 
   - Eliminación de puntuaciones, caracteres especiales y stopwords.
   - **Stemming** y **lemmatización** para reducir las palabras a su forma base.

2. **Tokenización**: 
   - División del texto en palabras individuales para analizar la frecuencia de aparición.

3. **Generación de la Nube de Palabras**: 
   - Se genera la nube de palabras con las palabras procesadas, destacando términos clave que rodean a personas mencionadas en el texto.

### Resultados
La nube de palabras mostró términos recurrentes que rodean a las personas en el corpus, proporcionando una visualización clara de los temas y palabras más utilizados. Las interacciones con las tres personas están mayormente centradas en palabras relacionadas con emociones positivas y peticiones específicas. Los términos "love" y "please" destacan significativamente, sugiriendo que las menciones son en su mayoría afectuosas, probablemente relacionadas con el apoyo incondicional de los seguidores. Además, la palabra "vote" aparece como un tema recurrente, lo que indica que gran parte de las interacciones están vinculadas a eventos o campañas donde se pide la participación activa de los seguidores.

### Conclusión:
Este análisis fue útil para identificar las palabras más comunes que rodean a las personas en un corpus textual, destacando términos clave y relaciones lingüísticas importantes. Esto facilita la interpretación de patrones de lenguaje y temas en el texto, lo que puede ser valioso para estudios lingüísticos o análisis de sentimiento.

---

## 2. Proyecto de Clasificación de Frutas y Verduras

### Descripción
El proyecto se enfoca en la clasificación de imágenes de frutas y verduras utilizando Redes Neuronales Convolucionales (CNNs). Se probaron tres arquitecturas: **MobileNetV2**, **VGG16** y **ResNet50**, siendo esta última la que mostró un mejor rendimiento en la tarea de clasificación.

### Bibliotecas Principales
- **TensorFlow & Keras**: Construcción y entrenamiento de modelos CNN.
- **OpenCV**: Carga y procesamiento de imágenes.
- **ImageDataGenerator**: Aumento de datos para mejorar la generalización del modelo.
- **Matplotlib & Seaborn**: Visualización de métricas y resultados.

### Pasos Realizados:
1. **Preprocesamiento de Datos**:
   - Las imágenes se redimensionaron a 224x224 píxeles y se normalizaron entre 0 y 1.
   - Se aplicaron técnicas de aumento de datos como **rotación**, **zoom** y **ajuste de brillo** para generar más variabilidad en el conjunto de entrenamiento.

2. **Entrenamiento del Modelo**:
   - Se entrenaron tres modelos: **MobileNetV2**, **VGG16** y **ResNet50**.
   - Los modelos se optimizaron utilizando **early stopping** y **reduce learning rate**.
   - **ResNet50** fue el modelo seleccionado debido a su precisión superior y estabilidad durante el entrenamiento.

3. **Evaluación del Modelo**:
   - Se evaluó el rendimiento de los modelos en función de la precisión y la pérdida.
   - La matriz de confusión mostró que **ResNet50** tuvo la mejor capacidad de predicción, con una precisión del 100% en casi todas las clases.

### Rendimiento de los Modelos
- **ResNet50**: Mostró el mejor rendimiento, alcanzando una precisión del 100% en el conjunto de validación, lo que indica su capacidad para generalizar bien en imágenes no vistas.
- **MobileNetV2** y **VGG16** también obtuvieron buenos resultados, pero fueron superados por ResNet50 en términos de precisión final.

### Conclusión:
**ResNet50** fue seleccionado como el mejor modelo debido a su alta precisión, estabilidad y capacidad de generalización. Su estructura más profunda y eficiente permitió un mejor manejo de la complejidad en la clasificación de imágenes de frutas y verduras, haciéndolo más robusto que MobileNetV2 y VGG16.

---

## Conclusión General:
Ambos proyectos destacaron la importancia del preprocesamiento de datos y la elección adecuada de modelos. En la nube de palabras, se pudieron identificar patrones clave en el uso del lenguaje alrededor de personas mencionadas. En la clasificación de imágenes, **ResNet50** demostró ser la mejor opción para manejar variaciones en imágenes y obtener una alta precisión en la tarea de clasificación.

---