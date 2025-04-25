# 📰 Fake News Detection using Machine Learning & Deep Learning

This project focuses on detecting fake news articles using both traditional machine learning and deep learning techniques. It aims to classify news articles as either **fake** or **real** based on their content.

## 📁 Project Structure

```

Fake_news_ML/
├── DeepLearning-FakeNewsDetection.ipynb  # Deep learning approach
├── FakeNewsDetection.ipynb               # Machine learning approach
├── Fake.csv                              # Dataset containing fake news articles
├── True.csv                              # Dataset containing real news articles
├── .gitignore                            # Git ignore rules
└── README.md                             # Project documentation
```


## 📊 Dataset Overview

The datasets used are `Fake.csv` and `True.csv`, each containing news articles labeled accordingly.

- **Fake.csv**: Contains fake news articles.
- **True.csv**: Contains real news articles.

Each dataset includes fields such as:

- **title**: The title of the news article.
- **text**: The full text of the news article.
- **subject**: The subject category of the news article.
- **date**: The publication date of the news article.

## ⚙️ Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/anish3565/Fake_news_ML.git
   cd Fake_news_ML
   ```


2. **Set up a virtual environment (optional but recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```


3. **Install the required packages:**

   Create a `requirements.txt` file with the necessary packages, such as:

   ```txt
   pandas
   numpy
   scikit-learn
   tensorflow
   keras
   nltk
   matplotlib
   seaborn
   ```


   Then install with:

   ```bash
   pip install -r requirements.txt
   ```


4. **Download NLTK resources:**

   Within the notebook or separately:

   ```python
   import nltk
   nltk.download('stopwords')
   nltk.download('punkt')
   ```


## 🧠 Machine Learning Workflow

The project includes two approaches:

### 1. Traditional Machine Learning (`FakeNewsDetection.ipynb`)

- **Data Preprocessing**: Cleaning text data, removing stop words, and tokenization.
- **Feature Extraction**: Using techniques like TF-IDF Vectorization.
- **Model Training**: Implementing algorithms such as Logistic Regression, Naive Bayes, and Support Vector Machines (SVM).
- **Evaluation**: Assessing model performance using metrics like accuracy, precision, recall, and F1-score.

### 2. Deep Learning (`DeepLearning-FakeNewsDetection.ipynb`)

- **Data Preprocessing**: Similar to the traditional approach with additional steps for deep learning models.
- **Model Architecture**: Building neural networks using Keras with layers such as Embedding, LSTM, and Dense.
- **Training**: Compiling and fitting the model with appropriate loss functions and optimizers.
- **Evaluation**: Analyzing model accuracy and loss over epochs, and evaluating on test data.

## 📈 Results

The models are evaluated based on their performance metrics. Typically, deep learning models may achieve higher accuracy but require more computational resources. The choice between traditional and deep learning approaches depends on the specific requirements and constraints of the application.

## 📌 Future Improvements

- Incorporate more advanced deep learning architectures like BERT for better context understanding.
- Implement real-time news article scraping and classification.
- Develop a user-friendly web interface for users to input news articles and receive classification results.

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

## 📬 Contact

For any questions or feedback, please contact [Anish](https://github.com/anish3565).
