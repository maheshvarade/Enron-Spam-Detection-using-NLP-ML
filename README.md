# Enron-Spam-Detection-using-NLP-ML
This project leverages the Enron email dataset to build a spam detection model using classical machine learning techniques. The model processes and classifies emails based on their subject lines and message bodies, with a final accuracy of 90–91% using Logistic Regression and Multinomial Naive Bayes classifiers.
 Dataset Overview
Original dataset size: 33,716 emails

Fields: Message_ID, Date, Subject, Message, Label

Message_ID and Date were retained for reference but not used in modeling.

Duplicates were removed based on Subject and Message content after cleaning.

Preprocessing Steps
✅ Subject Column:
Removed non-alphabetic characters.

Removed duplicate entries based on cleaned text.

✅ Message Column:
Similar cleaning as Subject (non-alphabetic character removal).

Duplicate messages removed after cleaning.

Final dataset size: 23,575 unique entries

Feature Extraction
Used CountVectorizer from scikit-learn to convert text into a Bag-of-Words representation.

Applied separately to both Subject and Message columns.


🤖 Models Used
Multinomial Naive Bayes

Logistic Regression

Both models were evaluated individually on:

Subject features

Message features

🏆 Achieved 90–91% accuracy on both fields using both models.

🚀 Future Improvements
Combine both Subject and Message features

Try TF-IDF instead of CountVectorizer

Experiment with deep learning models (e.g. LSTM, BERT)

