# Paralinguistic Feature Extraction for Audio Deepfake Detection
Bachelor Thesis 
Isabel Vrielink, May 2024

This repository contains the code and analysis for my Bachelor thesis, titled "Paralinguistic Feature Extraction for Audio Deepfake Detection Methods." The project introduces a novel approach to audio deepfake detection by leveraging paralinguistic feature extraction using the TRILLsson model developed by Google Research.

Project Overview
With the proliferation of deepfake technologies, detecting fraudulent audio samples has become increasingly complex. Traditional detection methods often focus solely on verbal content, overlooking non-verbal cues such as intonation, rhythm, and emotional tone. This thesis explores the potential of paralinguistic features to enhance the effectiveness of audio deepfake detection systems.

Key Contributions
•	Implemented TRILLsson, a state-of-the-art paralinguistic feature extraction model, to generate 1024-dimensional embeddings from audio samples.
•	Leveraged the ASVspoof2019 Logical Access dataset, consisting of over 80,000 audio samples, for training and evaluation.
•	Designed and trained a logistic regression model for binary classification between bona fide and spoofed audio samples.
•	Achieved a test accuracy of 97.9% and an Equal Error Rate (EER) of 3.04%, demonstrating the robustness of the proposed method.

Dataset
The ASVspoof2019 Logical Access dataset was utilized for this study. It comprises over 125,000 audio samples labeled as either bona fide (genuine) or spoofed. All audio clips were standardized to one second in length to ensure consistency during feature extraction and model training.

Methodology
1. Feature Extraction
Paralinguistic features were extracted using the TRILLsson model, generating 1024-dimensional embeddings for each audio clip.

2. Data Preprocessing
•	Labels were paired with embeddings, and the dataset was split into training (70%), validation (20%), and test (10%) subsets.
•	Applied StandardScaler for feature normalization.

3. Classification
Implemented a logistic regression model and trained it with an iteration limit of 10,000 to ensure convergence on the large dataset.

4. Evaluation
•	Metrics: Accuracy, Precision, Recall, F1-Score, and Equal Error Rate (EER).
•	Visualizations: Receiver Operating Characteristic (ROC) curve and Confusion Matrix.

Results
The logistic regression model demonstrated robust performance:
•	Test Set Accuracy: 97.9%
•	Precision: 90.5%
•	Recall: 89.4%
•	Equal Error Rate (EER): 3.04%
•	Area Under the ROC Curve (AUC): 0.99
These results underscore the potential of paralinguistic feature extraction as a promising method for future audio deepfake detection systems.

License
This repository is made available for viewing purposes only. No part of this repository, including but not limited to code, text, and analysis, may be used, modified, or distributed without explicit written permission from the author.
For permissions, please contact: isabelvrielink20@gmail.com.

References
•	TRILLsson Model: Google Research on Kaggle, https://www.kaggle.com/models/google/trillsson
•	Dataset: ASVspoof2019, https://www.asvspoof.org/index2019.html
•	Evaluation Techniques: Stack Overflow
•	Code for TRILLsson Processing: Provided by Superviser Prof. Dr. Eric Postma, Tilburg University

Contact
For inquiries or collaboration opportunities, please contact: isabelvrielink20@gmail.com.


