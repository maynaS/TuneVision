# TuneVision
Vision Transformer based Music Genre Classifier

## Directory Structure
```bash
├── Baseline
│   ├── Baseline.ipynb
│   ├── Ensemble.ipynb
│   ├── mfccs.json
│   └── SimpleCNN.ipynb
├── EDA
│   ├── BPM Boxplot.jpg
│   ├── Confusion Matrix.png
│   ├── Corr Heatmap.jpg
│   ├── EDA.ipynb
│   ├── Feature Importance.jpg
│   ├── PCA Scattert.jpg
│   └── xgb.model
├── Ensemble
│   └── Ensemble.ipynb
├── Experiments
│   ├── DeiT.ipynb
│   ├── ResNet18.ipynb
│   ├── SwinT.ipynb
│   └── ViT.ipynb
├── FeatureExtraction
│   └── FeatureExtraction.ipynb
├── LICENSE
├── MGC.yml
├── Output
│   ├── Baseline
│   │   ├── MFCC_CNN_acc_loss.png
│   │   └── MFCC_LSTM_acc_loss.png
│   ├── DeiT
│   │   ├── deit_accuracy.png
│   │   └── deit_loss.png
│   ├── ResNet18
│   │   ├── resnet18_accuracy.png
│   │   └── resnet18_loss.png
│   ├── SimpleCNN
│   │   ├── simplecnn_accuracy.png
│   │   └── simplecnn_loss.png
│   ├── SwinT
│   │   ├── swint_accuracy.png
│   │   └── swint_loss.png
│   └── ViT
│       ├── attention.png
│       ├── vit_accuracy.png
│       └── vit_loss.png
├── Preprocessing
│   └── Preprocessing.ipynb
├── README.md
├── RecommendorSystem
│   └── RecSys.ipynb
```

## Installation
1. Clone the repository
2. Download the dataset from [here](https://www.kaggle.com/andradaolteanu/gtzan-dataset-music-genre-classification)
3. Extract the dataset and place it in the Data folder
4. Run the notebooks

## Running the code
- First run the <b>Preprocessing</b> notebook to generate the train-validation-test split of features of the audio files for 3-second and 30-second intervals (using features_3_sec.csv and features_30_sec.csv). These features will be used to train and evaluate the ML models in other notebooks. The <b>Preprocessing</b> notebook also contains explanations and visual depictions of different time-domain and frequency-domain features that can be extracted and analyzed from the GTZAN audio files.
- The <b>FeatureExtraction</b> notebook can be run to generate the same time-domain and frequency-domain features, and generate mel-spectrograms.
- The <b>EDA</b> notebook contains analysis of the dataset and audio features, as well as feature importance and confusion matrix for XGB classifier model, and a comparison of accuracies of various ML models.
- The <b>RecSys</b> notebook is a simple implementation of a recommender based on cosine similarity using just the features (csv files) extracted earlier.
- The <b>Ensemble</b> notebook compares the performance of Swin Transformer and Resnet model individually and when combined into an ensemble classifier. The code also evaluates the accuracy of Cross Gradient Booster model.
- The <b>Baseline</b> notebook trains and evaluates CNN, LSTM and traditional ML models to assess their performance on the dataset.
- The <b>SimpleCNN</b> notebook trains and evaluates a simple custom CNN with 2 convolution layers. An analysis of genre-wise accuracy is also performed.
- The <b>Experiments</b> folder contains notebooks that train, test and evaluate Data Efficient Image Transformers, ResNet18 Model, Swin Transformers and Vision Transformers on the dataset. 


## Contributors
- [Sanyam Shah](https://github.com/maynaS)
- [Vikram Rao](https://github.com/viks01)
-[Venika Sruthi](https://github.com/venika-19)
