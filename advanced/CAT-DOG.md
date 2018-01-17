# Cat-Dog classification

It is for classification of the given image into cat and dog using Keras. We use keras with tensorflow as the backend.

You can find the environment configuration file as [tensorflow.yml](tensorflow.yml) file.

### Setting up the environment

Open up your terminal and run
```bash
conda env create -f tensorflow.yml
```

To activate the environment, after the environment has been created, run

For linux/macOs users:
```bash
source activate tensorflow
```

For Windows users:
```bash
activate tensorflow
```

## Dataset Download and Structure

### Dataset
The dataset can be downloaded from [fast.ai](http://files.fast.ai/data/) . Download the dogscats.zip file.

### Folder Structure

In the folder with the jupyter notebook, create a folder named dataset and inside the folder unzip the dogscats.zip file.

The structure of the folder should look like this:
advanced
└── dataset
    └── dogscats
        ├── sample
        │   ├── train
        │   │   ├── cats
        │   │   └── dogs
        │   └── valid
        │       ├── cats
        │       └── dogs
        ├── test1
        ├── train
        │   ├── cats
        │   └── dogs
        └── valid
            ├── cats
            └── dogs


