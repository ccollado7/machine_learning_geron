# Machine Learning - Aurélien Géron
This repository contains the development and practices corresponding to the book *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition*

>https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/


>The original repo withn notebooks are in https://github.com/ageron/handson-ml2


## Pre-requirements

* [git](https://git-scm.com/downloads)
* [anaconda](https://www.anaconda.com/products/individual) / [minconda](https://docs.conda.io/en/latest/miniconda.html)

### Steps

**Step 1**: Download the repository.

```bash
$ git clone https://github.com/ccollado7/machine_learning_geron.git
$ cd machine_learning_geron
```

**Step 2**: Create environment dependencies for the project (Stopped in the project directory).

```bash
$ conda env create -f environment.yml
```

**Step 3**: Activate the environment where the project dependencies are installed.

```bash
$ conda activate ml-geron
```

**Paso 4**: On the project directory we raise jupyter lab or jupyter notebook

```bash
$ jupyter lab

Jupyter Notebook 6.1.4 is running at:
http://localhost:8888/?token=45efe99607fa6......
```

**Step 5**: Go to http://localhost:8888.... as indicated in the console.

## Add a new dependency

**Step 1**: Add the new dependency to ´environment.yml´

Conda has its own package repositories but in case of any problems you can always use the pip packages.

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

**Step 2**: Once we add the name of the new package in ´environment.yml´ it remains to install it. For this we must **update** our environment with the changes we made in ´environment.yml´ as follows:

```bash
$ conda env update -f environment.yml
```
**Step 3**: Finally, if we had **jupyter lab** open, we must restart the kernel where our notebook is running in order to load the new library.

![image](https://user-images.githubusercontent.com/962480/145253730-365cb56b-ae26-41b0-a38d-41d505c9ea74.png)
