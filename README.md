# CA2 - Email Spam Classification using Gaussian Naive Bayes

## Project Overview
This project implements an email spam classification system using the Gaussian Naive Bayes machine learning algorithm. 
The objective of the program is to automatically classify emails as either spam or non-spam (ham) based on the frequency of words appearing in the email text. 
This project demonstrates a complete machine learning pipeline, including text preprocessing, feature extraction, model training, prediction, and performance evaluation.


## Motivation and Purpose
Email spam detection is a common and practical application of machine learning and text classification.
By applying the Naive Bayes algorithm, this project shows how probabilistic models can be used to efficiently and accurately classify text data with relatively simple feature engineering techniques.


## Technologies and Libraries Used
The project was implemented using the following tools and libraries:
- Python 3
- NumPy (for numerical computations and matrix operations)
- scikit-learn (for machine learning model training and evaluation)
- os (for directory and file handling)
- collections.Counter (for building the word frequency dictionary)


## Dataset Description
The dataset consists of email messages organized into two separate folders:
- `train-mails`: Contains labeled training emails
- `test-mails`: Contains labeled testing emails

Each email is stored as a text file. Spam emails are identified by filenames starting with `spmsg`, while non-spam emails use a different naming convention. 
The datasets are provided as compressed ZIP files and are extracted at the beginning of the notebook.


## Methodology
The program follows these main steps:
1. A dictionary of the top 3,000 most frequent words is constructed from the training email dataset.
2. Each email is converted into a numerical feature vector based on word frequency counts using the constructed dictionary.
3. A Gaussian Naive Bayes classifier is trained using the training feature matrix and corresponding labels.
4. The trained model predicts labels for the test email dataset.
5. Model performance is evaluated using classification accuracy.


## How to Run the Project
To run this project successfully, follow these steps:
1. Upload the Jupyter Notebook and the dataset ZIP files to Google Colab or a local Python environment.
2. Run the notebook cells to extract the training and testing email folders.
3. Execute the remaining notebook cells in order to perform feature extraction, model training, and evaluation.
4. Review the printed accuracy output to assess model performance.


## Results
The Gaussian Naive Bayes model achieves an accuracy of approximately 96% on the test dataset. 
This result demonstrates that the model is effective at distinguishing between spam and non-spam emails using a simple word frequency-based feature representation.


## Limitations and Future Improvements
Although the model performs well, it relies on basic word frequency features and does not consider word order or semantic meaning.
Future improvements could include using more advanced text preprocessing techniques, such as TF-IDF, n-grams, or alternative machine learning models.


## Acknowledgements
This project was completed as part of a machine learning coursework assignment. The implementation follows the structure and guidelines provided in the course materials.

