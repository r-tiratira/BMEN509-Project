# BMEN 509 Group Project

This is the repository for BMEN 509 group project.

Group #: L01- 1

Members:
- Sergiy Redko (30151178)
- Romanard Tiratira (30142708)

## Data

For this project we used brain MRI dataset from kaggle.

Source: https://www.kaggle.com/datasets/mateuszbuda/lgg-mri-segmentation/data

## Replicating the Experiments

All our code is contained in [`segmentation.ipynb`](./segmentation.ipynb) file. There are 2 way to run it:

1. Locally in this repository.
2. Via kaggle.

### Run Locally

We do not recommend this method as it may take hours to train our MLs locally.

1. Create and start the virtual environment:
    1. `python -m venv venv`
    2. `.\venv\Scripts\activate.bat`
2. Install all required modules with `pip install -r requirements.txt`.
3. Modify the location of data directory in Cell 8 (code default is for kaggle imports):
```python
data_dir = '/kaggle/input/lgg-mri-segmentation/kaggle_3m'
```
4. Run the notebook and wait.

### Run Via Kaggle

1. Log into [kaggle](https://www.kaggle.com/).
2. Create new notebook.
3. Import [`segmentation.ipynb`](./segmentation.ipynb) (File > Import > Select file...).
4. To speed up the training, we recommend enabling the acceleration (Settings > Accelerator > GPU P100). Please note, even with acceleration, this process will take around **an hour**.
5. Run the notebook.
