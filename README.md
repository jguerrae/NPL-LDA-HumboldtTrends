# Análisis de Tendencias Temáticas en Investigaciones del Instituto Humboldt

## Descripción General
Este repositorio contiene un script de Python diseñado para realizar un análisis exhaustivo de las tendencias temáticas en las investigaciones del Instituto Humboldt. A través de técnicas avanzadas de Procesamiento de Lenguaje Natural (PLN) y clustering, el script automatiza la extracción, análisis y visualización de datos a partir de abstracts de las investigaciones. Este enfoque sistematizado no solo facilita la comprensión de las áreas de enfoque científico del Instituto sino que también destaca la evolución de los temas de investigación a lo largo del tiempo.

## Pasos Clave del Proceso

### 1. Extracción de Enlaces
Recupera todos los enlaces relevantes de la página web del repositorio, utilizando expresiones regulares para filtrar los documentos de interés, como PDFs.

### 2. Descarga de Documentos
Descarga los archivos PDF filtrados y los almacena localmente, asegurando que cada documento se identifique y clasifique adecuadamente para análisis posteriores.

### 3. Extracción de Metadatos
Extrae metadatos esenciales (autor, fecha de publicación, resumen, etc.) utilizando `pandas` para organizar esta información en estructuras de datos tabulares.

### 4. Análisis y Organización de Datos
Implementa funciones de limpieza y reorganización de metadatos, preparando el conjunto de datos para un análisis detallado mediante modelos de aprendizaje automático.

### 5. Guardado de Resultados
Los resultados se almacenan en archivos Excel, proporcionando una base de datos estructurada de documentos y metadatos para futuros análisis e investigaciones.

## Procesamiento de Lenguaje Natural y Clustering

- **Preparación y Limpieza del Texto:** Elimina palabras innecesarias y normaliza el texto para prepararlo para el análisis.
- **Análisis de Tópicos con LDA:** Utiliza el modelo Latent Dirichlet Allocation (LDA) para identificar los temas predominantes dentro del corpus. El número de tópicos se optimiza buscando maximizar la coherencia del modelo, facilitando interpretaciones claras y relevantes.

$$
\text{LDA} \sim \sum_{k=1}^{K} \theta_{k} \cdot \phi_{k}
$$

- **Visualización:** Se generan nubes de palabras y heatmaps para visualizar la frecuencia y distribución de los tópicos. Además, se utilizan visualizaciones interactivas HTML con PyLDAvis para explorar los tópicos modelados.

## Resultados y Conclusiones

El script proporciona insights valiosos sobre las tendencias temáticas en las investigaciones del Instituto Humboldt, apoyando la toma de decisiones y el descubrimiento de conocimiento en el ámbito académico y de investigación. Los resultados destacan no solo las áreas de interés científico sino también cómo estas áreas han evolucionado a lo largo del tiempo.

## License
This project is licensed under the MIT License, allowing for usage, modification, and distribution under certain conditions.

### Contact
For questions or collaborations, please contact [Jorge Guerra](mailto:ja.guerrae@uniandes.edu.co)

