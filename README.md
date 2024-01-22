# Audio Classification using Feature Extraction
----------------------------------------------------------------------------------------------------------
Audio Classification Project
Overview
This project focuses on the classification of audio samples, specifically distinguishing between tram and car sounds in the Hervanta and city center region of Hervanta, Tampere. The dataset comprises 50 samples (25 trams and 25 cars) collected using mobile phones.

----------------------------------------------------------------------------------------------------------
Data Collection
Data collection involved direct recording of tram sounds in .wav format and conversion of car sounds to .wav format, which were then uploaded to freesound.org. The total dataset for training the model consists of 446 audio samples (217 tram, 229 car) sourced from freesound.org.

Car Data:  https://freesound.org/people/erfanmo/packs/37114/

Tram Data:  https://freesound.org/people/pikachu_bear/packs/37085/

----------------------------------------------------------------------------------------------------------
Feature Extraction

Various feature extraction methods were explored, with a focus on achieving high accuracy. Short-time Fourier Transform (STFT) and Mel-frequency cepstral coefficients (MFCCs) emerged as promising choices. STFT provides time-frequency representation, while MFCCs mimic the human auditory system's sound processing.

----------------------------------------------------------------------------------------------------------
Model Selection and Training

To handle the large parameter count in the feature set, a Neural Network (specifically, a Convolutional Neural Network - CNN) was chosen over SVM, Nearest Neighbor, and Linear Regression. CNNs excel in processing time-series data like audio signals, allowing them to learn relevant features efficiently.

Model: Convolutional Neural Network (CNN)
Training/Testing split: 80%/20%

----------------------------------------------------------------------------------------------------------
Model Evaluation

Evaluation Metrics:

  Accuracy:

    Overall: 98% on the combined dataset

    Specific class accuracy:

        Tram: 99%
  
        Car: 97%

The model was trained and tested using the dataset, achieving an impressive accuracy score of 98%. The decision to use MFCCs as the chosen feature for training the CNN model was based on superior performance compared to STFT.

----------------------------------------------------------------------------------------------------------
Testing and Results

The model was evaluated using the collected tram and car data, resulting in an accuracy score of 98%. Comparative testing between STFT and MFCCs revealed that the latter provided better accuracy (98% vs. 92%), solidifying the choice of MFCCs for training the CNN model.

----------------------------------------------------------------------------------------------------------
Conclusion

This project demonstrates the successful classification of tram and car sounds using a CNN model trained on MFCC features. The approach leverages insights from human hearing, emphasizing frequency-related features to achieve high accuracy. The "images" folder in the uploaded zip file includes relevant plots of the features used in the analysis.

----------------------------------------------------------------------------------------------------------
Feel free to explore the code and data in this repository to gain a deeper understanding of the project and its outcomes. Your feedback and contributions are highly appreciated.
