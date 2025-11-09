# music-genre-classification-bilstm-attention
the growing popularity of online music streaming platforms and large volume of music creates a need of effective genre classification.this proposed system successfully classifies music genre using hybrid CNN-BILSTM model enhanced with attention mechanism

📘 Overview

GENREFY is a deep learning–based system designed to automatically classify music into genres using advanced audio feature extraction and hybrid neural network architectures.
The project combines Convolutional Neural Networks (CNN) and Bidirectional Long Short-Term Memory (BiLSTM) with an Attention Mechanism, enabling the model to capture both spatial and temporal characteristics of audio signals.

Our proposed hybrid approach achieved an impressive 94% accuracy on the GTZAN dataset, outperforming traditional methods and several recent deep learning baselines.

🧠 Motivation

With the explosion of digital music platforms like Spotify and Apple Music, there is a growing demand for intelligent systems that can categorize, recommend, and personalize music. Traditional machine learning approaches using handcrafted features struggle with genre overlaps and complex patterns.
GENREFY leverages deep learning to overcome these limitations and deliver robust, scalable classification performance.

🧩 Dataset

Dataset Used: GTZAN Music Genre Dataset

Total Samples: 1000 audio tracks

Duration: 30 seconds each

Sampling Rate: 22,500 Hz

Genres (10): Blues, Classical, Country, Disco, Hip-Hop, Jazz, Metal, Pop, Reggae, Rock

Distribution: 100 tracks per genre

⚙️ Methodology
🧹 Preprocessing

Loaded all 10 genres from the GTZAN dataset.

Split each audio file into 3-second chunks.

Applied data augmentation (time stretching) to increase diversity.

Standardized features using StandardScaler.

Encoded genre labels into numeric format.

🎼 Feature Extraction

Extracted the following acoustic features:

Mel-Frequency Cepstral Coefficients (MFCCs)

Chroma Features

Mel-Spectrograms

Spectral Contrast

🧮 Model Architecture

Hybrid CNN + BiLSTM + Attention network.

CNN layers extract spatial (frequency-time) patterns.

BiLSTM layers capture temporal dependencies.

Attention mechanism focuses on important time–frequency components.

Hyperparameters optimized using Optuna.
🧾 Evaluation Metrics

Accuracy

Precision

Recall

F1-score

Confusion Matrix

Training/Validation loss & accuracy plots
  #RESULT

| Genre     | Precision | Recall | F1-Score |
| --------- | --------- | ------ | -------- |
| Blues     | 95%       | 88%    | 92%      |
| Classical | 85%       | 100%   | 92%      |
| Country   | 100%      | 95%    | 97%      |
| Disco     | 94%       | 97%    | 95%      |
| Hip-Hop   | 96%       | 86%    | 91%      |
| Jazz      | 87%       | 93%    | 90%      |
| Metal     | 94%       | 92%    | 93%      |
| Pop       | 93%       | 100%   | 96%      |
| Reggae    | 100%      | 97%    | 98%      |
| Rock      | 96%       | 93%    | 94%      |






