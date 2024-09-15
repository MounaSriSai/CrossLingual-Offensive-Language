
# Cross-Lingual Offensive Detection

## Project Overview
This project aims to detect offensive language across different languages, specifically focusing on Arabic and English. It utilizes machine learning classifiers to analyze the linguistic features and distinguish between offensive, hateful, and neutral language. The project explores cross-lingual training, where models trained in one language are tested in another.

## Key Features
- **Multilingual Dataset**: Involves both Arabic and English datasets.
- **Preprocessing**: Text data is cleaned, and stopwords are removed using NLP techniques.
- **Machine Learning Models**: Various classifiers such as Decision Tree, Random Forest, AdaBoost, and Gradient Boosting are implemented.
- **Cross-Lingual Training**: Models trained on Arabic data are tested on English data and vice versa.
- **Performance Evaluation**: Confusion matrices and classification reports are generated to evaluate model accuracy.

## Installation Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/MounaSriSai/CrossLingual-Offensive-Language.git
   ```
2. Navigate into the project directory:
   ```bash
   cd CrossLingual-Offensive-Language
   ```
3. Install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. **Data Preprocessing**:
   - Open the Jupyter Notebook for preprocessing the Arabic and English datasets.
   - You can use the following command to start Jupyter Notebook:
   - ``` bash
     jupyter notebook
     ```
   - In the notebook interface, run the cells in the respective notebooks for Arabic and English preprocessing.
   - Stopwords are removed, and text is converted to a suitable format for classification.
   - The processed datasets are saved as `processedArabic.csv` and `processedEnglish.csv`.

2. **Training and Testing**:
   - Once the data is preprocessed, open the training and testing notebook in Jupyter:
   - Run the cells to train models and test them on cross-lingual data.
   - The models include classifiers like Decision Trees, Random Forest, AdaBoost, and Gradient Boosting.
   - You can modify the code to use different classifiers like Decision Trees, AdaBoost, or Random Forest.

## Project Structure
- `Training using Arabic & Testing using English.ipynb`: Script for training of arabic and testing with english.
- `Training using English & Testing using Arabic.ipynb`: Script for training of english and testing with arabic.
- `Arabic and English Language Process.ipynb`: Data Preprocessing
- `L-HSAB.txt`: Arabic language dataset.
- `labeled_data.csv`: English language dataset.
- `processedArabic.csv`: Preprocessed Arabic dataset.
- `processedEnglish.csv`: Preprocessed English dataset.
- `requirements.txt`: List of dependencies.

## Models and Techniques Used
- **Text Preprocessing**: Using regex for text cleaning and `nltk` for stopword removal.
- **Label Encoding**: Converting categorical target variables into numerical format.
- **TF-IDF Vectorization**: Converting text data into numerical features using `TfidfVectorizer`.
- **PCA**: Dimensionality reduction using Principal Component Analysis (PCA).
- **Over-Sampling**: Handling class imbalances using Random OverSampling.
- **Classification Algorithms**: Decision Trees, Extra Trees, Random Forest, AdaBoost, Gradient Boosting, and Bagging classifiers are implemented.

## Results
The performance of the classifiers is evaluated through confusion matrices and classification reports for both the Arabic and English datasets. The results show the effectiveness of cross-lingual learning in identifying offensive content.

