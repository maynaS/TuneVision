# TuneVision
Vision Transformer based Music Genre Classifier

## Directory Structure
```bash
├── Baseline
│   └── Baseline.ipynb
├── Data
│   ├── features_30_sec.csv
│   ├── features_3_sec.csv
│   ├── genres_original
│   │   ├── blues
│   │   ├── classical
│   │   ├── country
│   │   ├── disco
│   │   ├── hiphop
│   │   ├── jazz
│   │   ├── metal
│   │   ├── pop
│   │   ├── reggae
│   │   └── rock
│   └── images_original
│       ├── blues
│       ├── classical
│       ├── country
│       ├── disco
│       ├── hiphop
│       ├── jazz
│       ├── metal
│       ├── pop
│       ├── reggae
│       └── rock
├── EDA
│   ├── BPM Boxplot.jpg
│   ├── Confusion Matrix.png
│   ├── Corr Heatmap.jpg
│   ├── EDA.ipynb
│   ├── Feature Importance.jpg
│   └── PCA Scattert.jpg
├── FeatureExtraction
│   └── FeatureExtraction.ipynb
├── LICENSE
├── Preprocessing
│   └── Preprocessing.ipynb
├── README.md
└── RecommendorSystem
    └── RecSys.ipynb
```

## Code Structure
- Baseline
- EDA: Exploratory Data Analysis on the GTZAN dataset
- Feature Extraction: Extraction of features from raw audio files using the librosa library
- Preprocessing: Preprocessing of the data with detailed explanations about the features
- Recommender System
Each directory contains Jupyter Notebook files that perform specific tasks.

### EDA
This notebook explores various audio features extracted for classification.
It includes a correlation heatmap and a box plot for genre distribution, providing valuable insights into dataset characteristics.
It also employs traditional machine learning algorithms like Naive Bayes, SGD, KNN, etc., to establish a crude baseline for the dataset.

### Preprocessing
This Jupyter Notebook covers loading audio files using the librosa library.
It explains features relevant to Music Genre Classification, laying a solid foundation for feature extraction and model training.
It covers aspects like pre-emphasis filtering, chromagram, Fourier transform, zero-crossing rate (ZCR), spectral properties, with visualizations of audio clips in each genre.

### Feature Extraction
This notebook extracts statistics (e.g., mean, standard deviation, etc.) about various time domain and frequency domain features from the audio files.
It utilizes the librosa library and converts these features, along with labels and file names, into a dataframe and eventually to a CSV file, similar to the features_30_sec CSV file from the GTZAN dataset.

### Baseline
This notebook implements VGG CNN and LSTM models, training them on spectrogram images from the GTZAN dataset.
It also trains a baseline CNN model with three convolutional layers, serving as a benchmark.
The test accuracies of these models are compared to assess performance.

### Recommender System
Rudimentary recommender system for demonstration purposes in the MIR domain.

