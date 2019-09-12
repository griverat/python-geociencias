# Python para Geociencias

El objetivo de este repositorio es dar una introducción en el uso de Python para las geociencias, especificamente en la implementación de algoritmos, manejo de datos y visualización tanto estática como interactiva.

## Comenzando

Los notebooks se podrán usar interactivamente sin necesidad de instalación gracias a Binder, solo tiene que hacer click en el botón de `Launch Binder` y esperar un momento hasta que todo este listo.

**Nota:** Todo lo que trabaje o modifique dentro de la sesión de Binder se perderá al cerrar la sesión. Si desea guardar el trabajo realizado deberá descargar el Notebook dirigiendose a `File > Download as > Notebook (.ipynb)` (para Jupyter Notebook) o dandole click derecho al Notebook y seleccionando `Download` (para Jupyter Lab)

### Instalación

#### Requisitos

- conda - Instalar desde Anaconda
- git

#### Instrucciones

Para usar los notebooks de manera local primero deberá descargar o clonar este repo usando

```bash
git clone https://github.com/DangoMelon/python-geociencias.git && cd python-geociencias
```

Al terminar la descarga, se encontrará dentro de la carpeta que contiene los archivos de este repo. Deberá instalar el entorno de trabajo especificado en el archivo `environment.yml` usando el comando `conda`

```bash
conda env create -f environment.yml
```

Una vez terminada la ejecución del comando anterior será capaz de activar el nuevo entorno de trabajo usando `conda`

```bash
conda activate pangeo
```

Sabrá si se encuentra dentro del nuevo entorno si en su terminal aparece el nombre del entorno de la siguiente manera: `(pangeo) user@hostname:~$`

Ahora deberá iniciar una sesión de JupyterLab ejecutando lo siguiente en una terminal.

```bash
jupyter-lab
```
