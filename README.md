# Python para Geociencias

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DangoMelon/python-geociencias/master?urlpath=lab/tree/Notebooks/)

El objetivo de este repositorio es dar una introducción en el uso de Python para las geociencias, especificamente en la implementación de algoritmos, manejo de datos y visualización tanto estática como interactiva.

## Comenzando

Los notebooks se podrán usar interactivamente sin necesidad de instalación local gracias a Binder, solo tiene que hacer click en el botón de `Launch Binder` y esperar un momento hasta que todo este listo.

**Nota:** Todo lo que trabaje o modifique dentro de la sesión de Binder se perderá al cerrar la sesión. Si desea guardar el trabajo realizado deberá descargar el Notebook dirigiendose a `File > Download as > Notebook (.ipynb)` (para Jupyter Notebook) o dandole click derecho al Notebook y seleccionando `Download` (para Jupyter Lab)

### Instalación

#### Requisitos

- conda - Instalar para su sistema operativo desde [Anaconda (Python 3)](https://www.anaconda.com/distribution/)
- git

#### Instrucciones

Para usar los notebooks de manera local primero deberá descargar o clonar este repo usando el siguiente comando en una terminal

```bash
git clone https://github.com/DangoMelon/python-geociencias.git && cd python-geociencias
```

Si desea usar `git` en Windows, deberá instalar git desde su [página oficial](https://git-scm.com/downloads) y luego ejecutar Git Bash desde donde podrá hacer uso del comando `git`.

Al terminar la descarga, se encontrará dentro de la carpeta que contiene los archivos de este repositorio. Deberá instalar el entorno de trabajo especificado en el archivo `environment.yml` usando el comando `conda`

```bash
conda env create -f environment.yml
```

Para el caso de Windows, al instalar Anaconda se agregará el `Anaconda Powershell Prompt` desde el cual podrá invocar el comando `conda`. Asegurarse de estar usando el shell correcto ya que el comando no será reconocido si usa Git Bash, Powershell o CMD y no agregó Anaconda al _path_ de su sistema al realizar la instalación.

Una vez terminada la ejecución del comando anterior, será capaz de activar el nuevo entorno de trabajo usando `conda`

```bash
conda activate pangeo
```

Sabrá si se encuentra dentro del nuevo entorno si en su terminal aparece el nombre del entorno de la siguiente manera: `(pangeo) user@hostname:~$`

El archivo `postBuild` contiene comandos que agregarán extensiones a nuestra instalación de Jupyter. Por defecto, el script usa `bash` asi que deberá tener este shell instalado.

```bash
sh postBuild
```

Tambien puede copiar el contenido del archivo `postBuild` y ejecutarlo directamente desde la terminal en caso no use bash.

Ahora podrá iniciar una sesión de JupyterLab mediante el siguiente comando

```bash
jupyter-lab
```

#### Actualización

Para actualizar los paquetes del entorno de trabajo deberá ejecutar el siguiente comando

```bash
conda env update -f environment.yml
```

## Nota

El entorno de trabajo instalado contiene un set de paquetes utiles para los trabajos que desee realizar, sientase libre de personalizar el contenido del mismo conforme vaya necesitando algunos paquetes más especializados.

Si desea instalar un paquete adicional, deberá consultar la documentación del mismo donde especifican las opciones de instalación. Sin embargo, la mayoría de paquetes pueden ser instalados mediante el siguiente comando

```bash
conda install -c conda-forge PKG-NAME
```

Donde `PKG-NAME` es el nombre del paquete que desea instalar y `-c conda-forge` especifica que el paquete sea instalado desde el canal `conda-forge` (recomendado)
