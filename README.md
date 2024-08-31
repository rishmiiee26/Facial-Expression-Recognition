## Facial Emotion Recognition (FER)

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/facial-emotion-recognition-state-of-the-art/facial-expression-recognition-on-fer2013)](https://paperswithcode.com/sota/facial-expression-recognition-on-fer2013?p=facial-emotion-recognition-state-of-the-art)


### Installation
To use this repo, create a conda environment using `environment.yml` or `requirements.txt`

```
# from environment.yml (recommended)
conda env create -f environment.yml

# from requirements.txt
conda create --name <env> --file requirements.txt
```
Download the offical [fer2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data) dataset, and place it in the outmost folder with the following folder structure `datasets/fer2013/fer2013.csv`

### Usage

To train your own version of our network, run the following

```
python train.py network=vgg name=my_vgg
```
To change the default parameters, you may also add arguments such as `bs=128` or `lr=0.1`. For more details, please refer to `utils/hparams.py`
