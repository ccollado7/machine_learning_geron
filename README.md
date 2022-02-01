# Machine Learning - Aurélien Géron
This repository contains the development and practices corresponding to the book *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition*

>https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/


>The original repo withn notebooks are in https://github.com/ageron/handson-ml2


## Pre-Requisitos

* [git](https://git-scm.com/downloads)
* [anaconda](https://www.anaconda.com/products/individual) / [minconda](https://docs.conda.io/en/latest/miniconda.html)

### Pasos

**Paso 1**: Descargar el repositorio.

```bash
$ git clone https://github.com/ccollado7/machine_learning_geron.git
$ cd dm-cyt-tp
```

**Paso 2**: Crear environment de dependencias para el proyecto (Parado en el directorio del proyecto).

```bash
$ conda env create -f environment.yml
```

**Paso 3**: Activamos el entorno donde se encuentran instaladas las dependencias del proyecto.

```bash
$ conda activate ml-geron
```

**Paso 4 **: Sobre el directorio del proyecto levantamos jupyter lab.

```bash
$ jupyter lab

Jupyter Notebook 6.1.4 is running at:
http://localhost:8888/?token=45efe99607fa6......
```

**Paso 5**: Ir a http://localhost:8888.... como se indica en la consola.

## Agregar una nueva depedencia

**Paso 1**: Agregar la nueva depedencia a ´environment.yml´

Conda tiene sus propios repositorios de paquetes pero en caso de tener algun problema siempre se puede usar los paquetes de pip.

```yaml
...
dependencies:
  - SOY_UN_PAQUETE_DE_CONDA
  - SOY_OTRO_PAQUETE_DE_CONDA
  - pip:
    - SOY_UN_PAQUETE_DE_PIP
    - SOY_OTRO_PAQUETE_DE_PIP
...
```

**Paso 2**: Una vez que agregamos el nombre del nuevo paquetes en ´environment.yml´ resta instalarlo. Para esto debemos **actualizar** nuestro environment con con los cambios que realizamos en ´environment.yml´ de la siguiente forma:

```bash
$ conda env update -f environment.yml
```
**Paso 3**: Finalmente si teniamos abierto **jupyter lab**, debemos reinifiar el kernel donde estemso corriendo nuestra notebook para poder cargar la nueva libreria.

![image](https://user-images.githubusercontent.com/962480/145253730-365cb56b-ae26-41b0-a38d-41d505c9ea74.png)
