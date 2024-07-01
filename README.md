# CUSSer
CUSSer - Culturally Sensitive Speech Emotion Recognition

# 1) Initialize Environment.
We reccomend using [anaconda](https://conda.io/projects/conda/en/latest/index.html) to manage your python environments. Install the requirements from the environment.yml file using the following.  

```bash
conda env create -f environment.yml
```

# 2) Download Datasets:
The central dataset we are using is the [CREMA-D](https://github.com/CheyneyComputerScience/CREMA-D) dataset, the demographic information `VideoDemographics.csv` is already included in the repo, the audio files need to be downloaded seperatly either from the [CREMA-D](https://github.com/CheyneyComputerScience/CREMA-D) repository using [git-lfts](https://git-lfs.com/) or from [Kaggle](https://www.kaggle.com/datasets/ejlok1/cremad), and put in a folder callsed `AudioWAV` with this repository as the root. 

# 3) Black Box Model:
(wav2vec_emotion_classifier.ipynb) - pretrained wav2vec transformer with classifier head fine-tuned on the emotion classification downstream task (CREMA-D, EmoDB, BanglaSER)

Required packages: transformers pytorch-lightning wandb interpret torch torchaudio librosa scikit-learn scipy matplotlib.pyplot pandas tqdm

Final models' checkpoints can be downloaded [here](https://drive.google.com/drive/folders/1xV35le3CAtyYFhMR-no34hkZeFNDx_Un?usp=sharing)

Ready dataframes with BB model predictions and Global Surrogate model predictions can be downloaded [here](https://drive.google.com/drive/folders/1ZVQa7fiQIlfr9nMKNVe9rhVBK5cEZ6Vo?usp=sharing)

# 4) Extract Feautures: 
