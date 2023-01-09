# Detector y contador de personas y vehíclos con Yolov7

Contribuyentes:
- Juan Manuel Medina Ramos (juanmamed)
- Diego Castellano Caballero (dcastellanoo)

Haciendo uso del detector de objetos Yolov7, el objetivo de esta propuesta es realizar un conteo de del número de coches, camiones, motocicletas, buses y personas pasan a través de ciertas zonas de un vídeo de una cámara de tráfico.

### Proceso para la reproducibilidad del desarrollo

En primer lugar, deberá crear un nuevo environment desde Anaconda Prompt que cuente con Python 3.9.15. Para ello deberá ejecutar el siguiente comando, donde ENV_NAME puede ser sustituido por un nombre de su elección:

```
conda create -n ENV_NAME python=3.9
```
Una vez haya concluido la ejecución del anterior comando, deberá activar el environment recién creado:

```
conda activate ENV_NAME
```
Se instalará algunos paquetes necesarios:

```
pip install numpy cython
```
Ahora, deberá situarse en la carpeta llamada “easy-yolov7-main” la cual se encuentra dentro del repositorio descargado en primer lugar. Para ello, puede utilizar el comando “cd”. Ya situado en la ruta del directorio “easy-yolov7-main”, deberá descargar los paquetes necesarios mediante el siguiente comando:

```
pip install -r requirements.txt
```
Probablemente, al ejecutar el anterior comando, reciba un código de error debido al paquete cython_bbox. Si esto le llega a ocurrir, se ha incluido una implementación de dicho paquete en el repositorio del trabajo y para instalarlo deberá ejecutar el comando:

```
pip install -e ../cython_bbox-0.1.3
```
Y tras este, de nuevo ejecute el comando:

```
pip install -r requirements.txt
```
Con esto ya tendría instalados todos los paquetes necesarios para la ejecución de la implementación del trabajo realizado con el objetivo de desarrollar la propuesta de detección y conteo de vehículos y personas. 
Necesitará descargar el vídeo objeto de estudio e incluirlo en el directorio del trabajo. Este último lo puede descargar desde el siguiente enlace de Dropbox: https://www.dropbox.com/s/o8h6kpwsggl3vak/traffic-video-1080.mp4?dl=0

Por último, queda descargarse los pesos del modelo yolov7-e6e, archivo el cual debe incluir en la carpeta “easy-yolov7-main” y que puede descargar en el siguiente enlace: https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-e6e.pt

En este momento, ya tendría todo lo necesario para ejecutar el Jupyter Notebook en el que se encuentra la implementación del trabajo, el cual se llama “TrabajoVC.ipynb”. Este puede ser ejecutado desde Visual Studio Code con el intérprete de Python del environment creado anteriormente.






