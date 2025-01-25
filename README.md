# Spam Correo Electronico

Este proyecto aborda la clasificación de correos electrónicos como spam o ham (no spam) utilizando el algoritmo Naive Bayes. Para este propósito, se utilizó procesamiento de lenguaje natural (NLP) para extraer características relevantes de los correos y construir un modelo eficiente de clasificación. La base de datos utilizada contiene un conjunto de correos electrónicos etiquetados, y el modelo fue entrenado para identificar si un correo es spam o no, basándose en el contenido del mensaje.

## Metodología
El desarrollo del proyecto se estructuró en varias fases clave, desde la preparación de los datos hasta la implementación y evaluación del modelo de clasificación:

### 1. Preparación de los Datos
Para abordar el problema de clasificación, se utilizó un conjunto de datos de correos electrónicos que contiene ejemplos de correos spam y ham (no spam). Este conjunto de datos incluye el texto completo de los correos, y la tarea consiste en clasificar cada mensaje según si es spam o no.

### Preprocesamiento de los Datos:
- Eliminación de texto irrelevante: Se eliminó información como firmas de correos, direcciones de correo electrónico, enlaces y caracteres especiales.
- Tokenización: El texto de cada correo se dividió en tokens (palabras individuales) para analizar el contenido.
- Eliminación de stopwords: Se eliminaron las palabras comunes como "el", "la", "de", etc., que no aportan valor significativo a la clasificación.
- Lematización: Las palabras se redujeron a su forma base (por ejemplo, "corriendo" se convirtió en "correr").

### 2. Modelo de Clasificación: Naive Bayes
Se utilizó el algoritmo Naive Bayes, un clasificador probabilístico basado en el teorema de Bayes y la suposición de independencia condicional entre las características (en este caso, las palabras). Este enfoque es especialmente eficaz para la clasificación de texto debido a su simplicidad y capacidad para manejar grandes volúmenes de datos de texto.

### 3. Entrenamiento del Modelo
El modelo fue entrenado utilizando los datos de correos electrónicos preprocesados, que fueron divididos en un conjunto de entrenamiento y un conjunto de prueba. El entrenamiento del modelo se realizó en el conjunto de entrenamiento, donde el algoritmo ajustó los parámetros para maximizar la probabilidad de clasificación correcta de los correos.

### 4. Evaluación del Modelo
Para evaluar la calidad del modelo, se utilizaron varias métricas clave:

- Precisión: La fracción de correos correctamente clasificados como spam entre todos los correos clasificados como spam.
- Recall: La fracción de correos correctamente clasificados como spam entre todos los correos que realmente son spam.
- F1-Score: La media armónica entre la precisión y el recall, que proporciona una evaluación más equilibrada del rendimiento del modelo.
