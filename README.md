# Desarrollo de un sistema de diagnóstico complementario para apendicitis pediátrica utilizando redes neuronales convolucionales: Un análisis de datos clínicos del Hospital St. Hedwig.

## Seminario de Analítica y Ciencia de Datos

## Estudiante
Alejandro Martínez Hernández

## Resumen
En el proyecto propuesto, se diseñará un sistema de diagnóstico médico complementario para la detección de apendicitis pediátrica, utilizando redes neuronales convolucionales y análisis de datos estructurados. Se dispondrá de una base de datos de ecografías del abdomen del Hospital St. Hedwig, enriquecida con anotaciones clínicas. Se empleará la técnica de transferencia de aprendizaje con modelos avanzados como MobileNetV2, ResNet-50, Inception y VGG16, ajustando la última capa para tres categorías diagnósticas. Se explorarán algoritmos para datos estructurados y se evaluará si la fusión de múltiples modelos mejora la precisión del diagnóstico.

Se tomó la decisión de analizar los datos estructurados y las imágenes separadamente y por ello se crearon dos archivos '.ipynb'. En ellos encontrará explicaciones del proceso que se hizo de análisis. Se aclara que en el archivo Procesamiento_de_imagenes.ipynb los códigos adentro se ejecutaron locamente para facilitar el manejo, limpieza y procesamiento de los datos.

## Contenido

- **Procesamiento_de_imagenes.ipynb:** Se encuentra los códigos junto a su respectiva explicación sobre el poqué y el cómo de su procesamiento. Para que los códigos corran se recomienda realizarlo localmente en archivos separados, tener las librerías que allí se usan instaladas y crear una estruuctura de carpetas igual a la que se encuentra en 'procesadas' dentro de 'us_images'. 
- **structured_data:** Contiene los datos estructurados del proyecto
- **us_images (carpeta):** Posee 2 carpetas
    1. ***originales:*** contiene todas las imágenes originales del estudio sin ningún cambio.
    2. ***procesadas:*** contiene las carpetas con las rutas que se especifican en los códigos. **Si se desea ejecutar los códigos de Procesamiento_de_imágenes.ipynb, se deebn cambiar las rutas que están dentro de la carpeta a los códigos, adicionalmente TODAS las carpetas deben estar vacías, pues al ejecutar los códigos estás se están llenando y vaciando continuamente**
- **Analisis_de_datos.ipynb:** Análisis de datos estructurados. Aquí se encuentra el código y las decisiones que se tomaron para elegir los datos estructurados de importancia. 

## Base de datos original
Si por algún motivo se desea ingresar a la base de datos original, se puede dirigir [AQUÍ](https://zenodo.org/records/7711412)