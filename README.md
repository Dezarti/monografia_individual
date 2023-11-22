# Desarrollo de un sistema de diagnóstico complementario para apendicitis pediátrica utilizando redes neuronales convolucionales: Un análisis de datos clínicos del Hospital St. Hedwig.

## Seminario de Analítica y Ciencia de Datos

## Estudiante
Alejandro Martínez Hernández

## Aclaración

El profesor solicitó una modificaciones en la tercera entrega. Como esta cuarta entrega se realizó con base en esa tercera, se recalca que los cambios hecho en la tercera se generaron en esta cuarta.

Se modificó el código para que este pudiese correr desde el notebook en cualquier maquina sin tenerle que hacer modificaciones en las rutas de los archivos. A continuación se muestra la estructura del proyecto una vez se haya corrido este notebook, pues la carpeta de "procesadas" solo aparecera despues de ello. 

Como se podrá notar, la carpeta "originales/" está vacía por problemas en la carga de archivos a github. El lector puede descargar la [Base de Datos Original](https://zenodo.org/records/7711412), copiar y finalmente pegar las 2098 imágenes de "US_Pictures/" en "us_images/originales/" para ejecutar el notebook Procesamiento_de_imagenes.ipynb con todo el dataset. 

```
datos_monografia/
├─ README.md
├─ documentos/
│  ├─ G18 - ME04 - Alejandro Martínez Hernández.docx
├─ src/
│  ├─ Procesamiento_de_imagenes.ipynb
│  ├─ Analisis_de_datos.ipynb
├─ data/
│  ├─ structured_data/
│     ├─ app_data.xlsx
│  ├─ us_images/
│     ├─ originales/
│     ├─ procesadas/
│        ├─ ordenadas/
│           ├─ con_info/
│           ├─ no_apendice/
│           ├─ no_paciente/
│        ├─ selection/
│           ├─ con_info/
│           ├─ no_apendice/
│           ├─ no_paciente/
```

## Resumen
En el proyecto propuesto, se diseñará un sistema de diagnóstico médico complementario para la detección de apendicitis pediátrica, utilizando redes neuronales convolucionales y análisis de datos estructurados. Se dispondrá de una base de datos de ecografías del abdomen del Hospital St. Hedwig, enriquecida con anotaciones clínicas. Se empleará la técnica de transferencia de aprendizaje con modelos avanzados como MobileNetV2, ResNet-50, Inception y VGG16, ajustando la última capa para tres categorías diagnósticas. Se explorarán algoritmos para datos estructurados y se evaluará si la fusión de múltiples modelos mejora la precisión del diagnóstico.

Se tomó la decisión de analizar los datos estructurados y las imágenes separadamente y por ello se crearon dos archivos '.ipynb'. En ellos encontrará explicaciones del proceso que se hizo de análisis. Se aclara que en el archivo Procesamiento_de_imagenes.ipynb los códigos adentro se ejecutaron locamente para facilitar el manejo, limpieza y procesamiento de los datos.

## Contenido

### Nota: Esta era la estructura anterior antes de hacer las modificaciones solicitadas por el profesor en la tercera entrega.
- **G18 - ME04 - Alejandro Martínez Hernández**: Documento correspondiente al cuarto momento evaluativo. Se encuentra dentro de la carpeta 'documentos'.
- **Procesamiento_de_imagenes.ipynb:** Se encuentra los códigos junto a su respectiva explicación sobre el poqué y el cómo de su procesamiento. Para que los códigos corran se recomienda realizarlo localmente en archivos separados, tener las librerías que allí se usan instaladas y crear una estruuctura de carpetas igual a la que se encuentra en 'procesadas' dentro de 'us_images'. 
- **structured_data:** Contiene los datos estructurados del proyecto
- **us_images (carpeta):** Posee 2 carpetas
    1. ***originales:*** contiene todas las imágenes originales del estudio sin ningún cambio.
    2. ***procesadas:*** contiene las carpetas con las rutas que se especifican en los códigos. **Si se desea ejecutar los códigos de Procesamiento_de_imágenes.ipynb, se deebn cambiar las rutas que están dentro de la carpeta a los códigos, adicionalmente TODAS las carpetas deben estar vacías, pues al ejecutar los códigos estás se están llenando y vaciando continuamente**
- **Analisis_de_datos.ipynb:** Análisis de datos estructurados. Aquí se encuentra el código y las decisiones que se tomaron para elegir los datos estructurados de importancia. 

## Base de datos original
Si por algún motivo se desea ingresar a la base de datos original, se puede dirigir [AQUÍ](https://zenodo.org/records/7711412)