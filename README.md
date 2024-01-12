# Final-VC

Bienvenido al proyecto final, donde presentamos una suite de herramientas de procesamiento de imágenes diseñadas para abordar diversas necesidades visuales. Este conjunto de tres programas únicos combina la potencia de la programación y la visión por computadora para ofrecer soluciones a distintos problemas carácteristicos de este ámbito. A continuación, te presentamos una breve descripción de cada programa:

# Generador de Panoramas

Este script en Python une imágenes de diferentes carpetas para crear imágenes panorámicas utilizando la biblioteca OpenCV.

## Prerrequisitos
Asegúrate de tener lo siguiente instalado:
- Python
- OpenCV

## Configuración
1. Clona el repositorio.
2. Asegúrate de que la carpeta `Images` contenga subcarpetas con imágenes para unir.

## Uso
1. Ejecuta el script.
2. El script iterará a través de cada subcarpeta en la carpeta `Images`.
3. Para cada subcarpeta, lee las imágenes, las une y muestra la panorámica resultante.
4. Si la generación de la panorámica es exitosa, se mostrará en una ventana con el nombre de la subcarpeta.

### Parámetros
- `mainFolder`: La carpeta principal que contiene subcarpetas con imágenes.
- `max_width`: Ancho máximo de la panorámica generada.
- `max_height`: Altura máxima de la panorámica generada.

## Nota Importante
Asegúrate de que las imágenes en cada subcarpeta sean adecuadas para unir en una panorámica. Ajusta los parámetros `max_width` y `max_height` según tus preferencias.

Siéntete libre de experimentar con diferentes imágenes y estructuras de carpetas para obtener resultados variados.

**Nota:** El script utiliza la biblioteca OpenCV, así que asegúrate de instalarla con `pip install opencv-python` si aún no lo has hecho.

# Colorear Imágenes en Blanco y Negro

Este script de Python utiliza el poder de la inteligencia artificial y la visión por computadora para agregar color a imágenes en blanco y negro. La herramienta utiliza un modelo de red neuronal profunda para predecir y aplicar colores realistas a las imágenes de escala de grises.

## Guía de Uso

### Requisitos Previos
Asegúrate de tener instaladas las siguientes bibliotecas de Python antes de ejecutar el script:

- NumPy
- OpenCV

Puedes instalar estas bibliotecas utilizando el siguiente comando:

`pip install numpy opencv-python`

# Configuración
1. Descarga el modelo de la carpeta proporcionada en la variable `DIR`.
2. Asegúrate de tener una carpeta (`Images_BlackWhite`) con las imágenes en blanco y negro que deseas colorear.

## Uso
1. Ejecuta el script.
2. El programa cargará el modelo de colorización y procesará cada imagen en la carpeta especificada.
3. Las imágenes originales y sus versiones coloreadas se mostrarán en ventanas separadas.
4. Presiona cualquier tecla para pasar a la siguiente imagen o cierra la ventana para finalizar el proceso.

## Notas
- El modelo utilizado para la colorización se encuentra en la carpeta `model`. No es necesario modificarlo, pero asegúrate de que las rutas en el script coincidan con la ubicación de los archivos en tu sistema.
- Las imágenes coloreadas se muestran en ventanas redimensionadas para facilitar la visualización.

# Traductor de Lengua de Signos

Este script en Python utiliza la biblioteca MediaPipe y un modelo preentrenado de TensorFlow/Keras para traducir gestos de lengua de signos a texto. El script captura la alimentación de video en tiempo real desde la cámara web, detecta puntos clave utilizando el modelo holístico de MediaPipe y predice la acción correspondiente de lengua de signos utilizando un modelo de aprendizaje profundo cargado.

## Requisitos

- OpenCV (cv2)
- NumPy (numpy)
- MediaPipe (mediapipe)
- TensorFlow (tensorflow)
- Matplotlib (matplotlib)

Instala las bibliotecas necesarias utilizando el siguiente comando:

`pip install opencv-python numpy mediapipe tensorflow matplotlib`

##  Uso

- Asegúrate de que las bibliotecas necesarias estén instaladas.
- Descarga el modelo preentrenado (action.h5) y colócalo en el mismo directorio que el script.
- Ejecuta el script.
- La alimentación de video de la cámara web se mostrará con puntos clave superpuestos y predicciones en tiempo real. Las acciones de lengua de signos detectadas se mostrarán como texto en la pantalla.

##  Instrucciones

- El script utiliza puntos clave faciales, de postura y de manos para reconocer gestos de lengua de signos.
- Los gestos detectados se clasifican en acciones predefinidas como 'hello', 'thanks' y 'iloveyou'.
- Las predicciones se muestran en tiempo real, y las acciones reconocidas se muestran como texto en la pantalla.
- La frase reconocida se actualiza en función de las predicciones recientes.

##  Notas

- Asegúrate de que tu cámara web esté conectada y accesible para el script.
- El script utiliza el modelo action.h5 para la clasificación de acciones de lengua de signos. No modifiques el modelo a menos que sea necesario.
- Presiona 'q' para salir de la aplicación.

