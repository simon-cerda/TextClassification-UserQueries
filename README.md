# Proyecto de Clasificación de Texto

## Descripción General
Este proyecto consiste en la implementación de un modelo de clasificación de texto que predice si un mensaje está preguntando por la dirección del centro médico o no. Utiliza tecnicas de NLP para preparar los datos y modelos de ML para realizar las predicciones.

## Implementación

### Preprocesamiento de Datos
- **Limpieza de Texto**: Se realizó una limpieza inicial del texto, eliminando stop words.
- **Tokenización y Lemmatización**: Se tokenizó el texto en palabras individuales y se aplicó lemmatización para reducir las palabras a su forma base, usando la biblioteca `spaCy` para soportar el texto en español.
- **Vectorización**: Se transformó el texto en vectores numéricos utilizando `TfidfVectorizer` de `scikit-learn`
- Se aplicó **Oversampling** a la clase minoritaria para abordar el desequilibrio de clases en el conjunto de datos.
  
### Modelado
- Se experimentó con varios modelos, incluyendo **Regresión Logística** y **Random Forest**

### Evaluación
- Se utilizaron métricas como **precisión**, **recall** y **F1 score** para evaluar los modelos, dada la naturaleza desequilibrada del conjunto de datos.

## Suposiciones
- **Calidad de los Datos**: Se asumió que los datos estaban relativamente limpios y que la etiqueta proporcionada era precisa.
- **Representatividad**:  Se supuso que el conjunto de datos era representativo

## Mejoras Futuras
- **Optimización de Hiperparámetros**
- **Explorar mensajes predecidos incorrectamente**
- **Expansión del Conjunto de Datos**
- **Técnicas Avanzadas de NLP**
