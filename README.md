# A Generic Deepleaning project template

This template project uses python modularization to create a generic deeplearning project. The project is divided into 3 main modules: data, models and trainers. The data module contains the data loaders and the data processing pipeline. The models module contains the model architectures. The trainers module contains the training and evaluation loops. The project is configured using a mate.json file. The experiment module contains the code to run the experiments. The experiments are configured using a experiment file. By defualt you can run python experiments using a command such as:

```
python -m my-project.experiments.cnn.resnet18
```

To use json, yaml or toml files to configure the experiments, you can use the following command:

```
pip install yerbamate
```

Then you can run the experiments using a command such as:

```
mate train cnn resnet18
```


## File Structure

```
├── my-project
│   ├── data
│   │   ├── __init__.py
│   │   ├── loaders
│   │   │   ├── cifar
│   │   │   ├── __init__.py
│   │   │   └── mnist
│   │   │       └── __init__.py
│   │   └── preprocessing
│   │       └── __init__.py
│   ├── experiments
│   │   ├── experiment
│   │   │   └── __init__.py
│   │   └── __init__.py
│   ├── __init__.py
│   ├── models
│   │   ├── cnn
│   │   │   └── __init__.py
│   │   ├── __init__.py
│   │   └── vit
│   │       └── __init__.py
│   └── trainers
│       ├── classifier
│       │   └── __init__.py
│       └── __init__.py
└── README.md

13 directories, 14 files
```