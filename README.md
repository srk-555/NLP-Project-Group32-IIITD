# NLP-Project-Group32-IIITD
Group 32 NLP Project Repo, IIIT Delhi
Group Members:
Amey Pawar, MT22010
Shreeyash Khalate, MT22069
Swaib Ilias Mazumder, MT22078
Rahul Malik, 2021554

Imports and Setup:
Importing necessary libraries like pandas, numpy, nltk, etc.
Installing required packages using pip install commands.
Loading language models like 'en_core_web_sm' from spaCy.

Data Preprocessing:
Reading the training dataset (F2_Claim_Check_Worthiness_train.csv) into a pandas DataFrame.
Preprocessing the text data, including:
Removing white spaces, lowercasing, and tokenization.
Removing stopwords, punctuation, URLs, and HTML tags.
Spell checking using the autocorrect library.
Saving the preprocessed data into a new CSV file (preprocessed_train.csv).

Feature Extraction:
Extracting features such as parts of speech (POS) tags and dependency relations.
Calculating the occurrence count of unique dependencies in the dataset.
Identifying the most important dependencies based on their occurrence count.

Data Transformation:
Scaling the extracted features using MinMaxScaler.
Applying Principal Component Analysis (PCA) for dimensionality reduction.

Modeling:
Using the SentenceTransformer library to obtain sentence embeddings.
Building a pipeline for data transformation and model training.
Splitting the preprocessed data into training and validation sets.
Training a Support Vector Machine (SVM) model on the training data.
Evaluating the model's performance using macro F1-score on both train and test sets.

Predictions:
Making predictions on the test dataset (F2_Claim_Check_Worthiness_test.csv) using the trained SVM model.
Saving the predictions along with their corresponding IDs into a CSV file (output5.csv).

Evaluation:
Computing and displaying a confusion matrix and a classification report for the model's performance on the validation set.
