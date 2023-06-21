# Sentimental Analysis
![moringa_phase4_project](https://github.com/Daniel1999Akama/moringa_phase4_project/assets/127243987/44675d35-58cc-411a-baa7-c3422ebfcd75)

## Table of Contents

- Sentimental Analysis
- Project Overview 
- Problem Statement 
- Data Understanding
- Methodology
- Evaluation
- Conclusion
- Recommendation
- Next Steps
- Installation
- Collaborators
- Repository Structure 

# Business understanding
In today’s digital age, social media platforms such as Twitter have become powerful sources of real-time customer feedback and opinions. Understanding the sentiment expressed by customers toward specific brands and products is essential for businesses to make informed decisions, enhance customer satisfaction, and maintain a positive brand reputation. 

The goal of this project aims to develop a sentimental analysis model specifically tailored to analyze Twitter data related to Google, Apple, and other products. 

# Business Problem Statement

As a consulting firm, Twitter has assigned us the task of building a model that can rate the sentiment of a Tweet based on its content  that can correctly categorize Twitter sentiment about Apple and Google products into positive, negative, or neutral categories and  gain valuable insights into public perception, that will be used for informed decision-making in business strategies and customer satisfaction enterprise.


# Data understanding
In this project, we analyze sentiment using a dataset of customer reviews collected from Twitter. The dataset contains a collection of text reviews and corresponding sentiment labels indicating whether the sentiment expressed in the review is positive, negative, or neutral. The dataset consists of 9093 rows and 3 columns.

To gain a better understanding of the data, we performed the following steps:

Data Collection: We collected the customer data world where there is a data set from from twitter platforms and review aggregators. The reviews were selected based on relevance to our analysis.

Data Preprocessing: We cleaned the raw text data by removing any irrelevant information, such as HTML tags, URLs, and special characters. We also performed tokenization, stop word removal, and stemming/lemmatization to normalize the text.

Exploratory Data Analysis (EDA): We conducted an in-depth analysis of the dataset to uncover patterns, trends, and insights. This included analyzing the distribution of sentiment labels, examining the most frequent words, and exploring any relationships between sentiment and other variables.

Data Visualization: We used various visualization techniques, such as bar plots, and sentiment distribution charts, to visually represent the data and gain further insights into the sentiment patterns.

## Project Overview
The objective of this project is to develop a sentiment analysis model that can accurately classify customer reviews into positive, negative, or neutral sentiment categories. The model aims to automate the process of sentiment classification, enabling businesses to quickly understand customer sentiment at scale.
To achieve this, we implemented the following steps:
1. Data Preparation: We split the dataset into training and testing sets to evaluate the performance of our model. We used X% of the data for training and Y% for testing.
2. Feature Extraction: We applied various techniques such as bag-of-words, count vectorizer 
3. Model Selection: We experimented with different algorithms, such as logistic regression. We evaluated the models using appropriate evaluation metrics such as accuracy.
4.Model Training and Evaluation: We trained the selected model on the training data and evaluated its performance on the testing data.
5. Model Deployment: Once we achieved satisfactory performance, we deployed the sentiment analysis model to make predictions on new, unseen customer reviews. using streamlit library.
By undertaking this project, we aim to provide businesses with valuable insights into customer sentiment, enabling them to make data-driven decisions, improve customer satisfaction, and enhance their overall brand reputation.
Please note that the above example is just a brief illustration, and you should customize it according to your specific project requirements and scope.

Methodology
Data Preprocessing: We performed data cleaning and preprocessing steps such as removing special characters, stopwords, and performing tokenization. We also applied lemmatization using NLTK's lemmatizer to reduce words to their common root form.

Vectorization Techniques:
a. Bag-of-Words (CountVectorizer): We used sklearn's CountVectorizer to convert the text data into a numerical representation, capturing the frequency of words in each document. This approach creates a matrix of word counts.

b. Classification Models: We trained and evaluated several classification models using the vectorized data, including:

1.Logistic Regression Classifier for the binary classifier model

2.Multinomial Naive Bayes and XGBoost model for the multiclass classification model 

c. Model Evaluation: For each model, we employed  accuracy to evaluate the model's ability to correctly predict sentiment.

d. Handling Class Imbalance: we tried to address this issue using synthetic Minority random Undersampling but didnt improve the accuracy of the XGBoost model.

# Evaluation
To evaluate the performance of our NLP sentiment analysis model, we conducted thorough testing and analysis using various evaluation metrics. The following evaluation results provide insights into the effectiveness of our approach:
* Accuracy:
1. Our binary sentiment analysis model achieved an overall accuracy of 90% which surpused our trget of achieving 85%.
2. our MultinomialNb multiclass model achieved an overall accuracy of 65%
3. our XGboost multiclass model achieved an overall accuracy of 68%


![image](https://github.com/Daniel1999Akama/moringa_phase4_project/assets/96378206/158e9d2a-3fe3-4f45-ab69-3831220f3aae)

No emotion towards brand had the highest value count 

# Findings
Most of the tweets were directed to no specific brand.
Positive sentiments had the highest count compared to Negative sentiments, indicating that most people in general liked respective brands(Google and Apple)
Most of the positive tweets were directed to Apple brands
In the field of sentiment analysis, one of the significant challenges is dealing with language ambiguity and sarcasm detection. Natural language is complex and often subjective, making it difficult to accurately interpret sentiments from text.
On average most of the tweets were 10-15 words long - more words increase ambiguity.
NLP is a difficult task to model accurately.
Most tweets were directed to None brand category. This may indicate that customers were not engaging with the brand.

# Recommendations
We recommend that there be more customer engagement.
Probably check on this areas;
Churn ratio - rate at which customers discontinue their relationship with a product company within a given time period
Social media influencers through brand or product endorsement
Customer feedback - The brands can introduce a rating system to accurately capture the sentiments of their customers

# Nextsteps
1. In our future work, we plan to explore advanced techniques such as incorporating attention mechanisms, using ensemble methods to further enhance the model's performance by incorporating domain-specific and fine-tuning the model on industry-specific datasets could improve its accuracy and adaptability.
2. By considering these evaluation metrics, addressing limitations, and planning for future improvements, we aim to develop a robust NLP sentiment analysis solution that effectively captures sentiment in text data.
3. Looking for a better dataset 


# Limitations
- Class Imbalance Issue: The dataset suffers from class imbalance, where one sentiment class is dominant while others are underrepresented. This can result in biased models that are more accurate for the majority class but perform poorly on the minority classes. Addressing this issue is important to ensure fair and balanced sentiment analysis.
- Limited Dataset Size: The dataset used for sentiment analysis is relatively small, which can limit the model's ability to capture the full complexity of sentiments expressed in text. A larger and more diverse dataset would provide a broader representation of sentiments and improve the model's performance and generalization.
- Language Ambiguity and Sarcasm Detection: Language can be inherently ambiguous, and detecting sarcasm in text adds an extra layer of complexity. Sarcasm detection is challenging due to the subtleties and nuances involved. Developing robust strategies to handle language ambiguity and detect sarcasm is crucial for accurate sentiment analysis

# Installations
To install and run this project, follow these steps:
1. Clone the repository to your local machine using the following command:
    - git clone https://github.com/Daniel1999Akama/moringa_phase4_project.git
2. Navigate to the project's root directory:
    - cd your-repository
3. Install the project dependencies(For this project we worked with Jupyter notebook, however it can also run on vscode or Google collab:
    - This command will install all the necessary packages and libraries required for the project to run(this should br run in the terminal(for our case Anaconda).
    - pip install Jupyter Notebook 
5. Call the note book in the directory
    - jupyter notebook
    - code .. for VS code
6. Open your web browser and access the application at http://localhost:5000.
    This is the default URL where the application will be running locally. 

### Collaborators
feel free  to visit this jupyternotebook and contact below emails


Rosemary Nyakio: @nyakio19roseary@gmail.com

Maureen Anduuru: @moesaitia@gmail.com

Daniel Akama: @danielakama23@gmail.com

Leah Katiwa: @katiwaleah26@gmail.com

Lynne mutwiri: @mutwirilyneek@gmail.com

Brian Nderu: @briannga00@gmail.com



### Repository Structure: 

├── .gitignore                                              

├── CONTRIBUTING                                            

├── LISENCE.md                                             

|── Phase4_project.ipynb                                   

├── data                                                   

├── README.md                                             



