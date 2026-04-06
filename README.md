<h1>News Topic Classification</h1>
<h2>Overview</h2>
<p>This project focuses on classifying news articles into predefined categories using Natural Language Processing (NLP) and Machine Learning techniques. 
The goal is to automatically categorize news content into topics such as World, Sports, Business, and Science/Technology based on textual data.</p>
<p>The model analyzes patterns in news headlines and descriptions to learn distinguishing features that define each category.</p>

<h2>Objective</h2>
<ul>
  <li>Classify news articles into multiple categories</li>
  <li>Build a complete NLP pipeline for multi-class classification</li>
  <li>Understand feature extraction using TF-IDF</li>
  <li>Evaluate model performance using standard metrics</li>
</ul>

<h2>Dataset</h2>
<p>The dataset consists of two files:</p>
<ul>
  <li><b>train.csv</b> - Used to train the model</li>
  <li><b>test.csv</b> - Used to evaluate model performance</li>
</ul>
<ul>
  <li>Title of the news article</li>
  <li>Description of the news article</li>
  <li>Class Index representing the category</li>
</ul>
<p>Category Mapping:</p>
<ul>
  <li>1 - World</li>
  <li>2 - Sports</li>
  <li>3 - Business</li>
  <li>4 - Science/Technology</li>
</ul>
<p>Dataset Link: https://www.kaggle.com/datasets/amananandrai/ag-news-classification-dataset</p>

<h2>Tech Stack</h2>
<ul>
  <li>Python</li>
  <li>Pandas, NumPy</li>
  <li>Matplotlib</li>
  <li>Scikit-learn</li>
  <li>Natural Language Processing (NLP)</li>
</ul>

<h2>Data Preprocessing</h2>
<p>To improve model performance, the following preprocessing steps were applied:</p>
<ul>
  <li>Combined title and description into a single text field</li>
  <li>Converted text to lowercase</li>
  <li>Removed URLs</li>
  <li>Removed special characters and punctuation</li>
  <li>Stored cleaned text for further processing</li>
</ul>
<p>These steps ensure consistency and reduce noise in the dataset.</p>

<h2>Exploratory Data Analysis (EDA)</h2>
<p>Basic analysis and visualizations were performed to understand the dataset:</p>
<ul>
  <li>Distribution of news categories</li>
  <li>Text length distribution</li>
  <li>Inspection of cleaned versus original text</li>
</ul>
<p>This helped in understanding the structure and balance of the dataset.</p>

<h2>Feature Engineering</h2>
<h3>TF-IDF Vectorization</h3>
<p>The textual data was converted into numerical form using TF-IDF (Term Frequency–Inverse Document Frequency):</p>
<ul>
  <li>Transforms text into numerical feature vectors</li>
  <li>Highlights important words based on their relevance</li>
  <li>Reduces the impact of commonly occurring words</li>
</ul>
<p>This allows the machine learning model to interpret textual input effectively.</p>

<h2>Model Building</h2>
<h3>Algorithm Used: Logistic Regression</h3>
<ul>
  <li>Supervised learning algorithm suitable for multi-class classification</li>
  <li>Efficient for large datasets</li>
  <li>Performs well with high-dimensional sparse data</li>
</ul>
<p>The model was trained on TF-IDF-transformed features to classify news articles into categories.</p>

<h2>Model Evaluation</h2>
<p>The model was evaluated using the following metrics:</p>
<ul>
  <li><b>Accuracy Score</b> to measure overall correctness</li>
  <li><b>Confusion Matrix</b> to analyze prediction performance</li>
  <li><b>Classification Report</b> including:
    <ul>
      <li>Precision</li>
      <li>Recall</li>
      <li>F1-score</li>
    </ul>
  </li>
</ul>
<p>These metrics provide a comprehensive evaluation of the model across all categories.</p>

<h2>Visualizations</h2>
<h3>Category Distribution</h3>
<p>Shows how data is distributed across different news categories.</p>
<img src="https://github.com/IshitaSinha2002/News-Topic-Classifier/blob/main/Confusion%20Matrix.png" width: 500px; height: 400px; object-fit: cover;>
<h3>Confusion Matrix</h3>
<p>Displays actual versus predicted classifications.</p>
<img src="https://github.com/IshitaSinha2002/News-Topic-Classifier/blob/main/News%20Topic%20Dist.png" width: 500px; height: 400px; object-fit: cover;>
<h3>Text Length Distribution</h3>
<p>Shows variation in the length of news articles.</p>
<img src="https://github.com/IshitaSinha2002/News-Topic-Classifier/blob/main/Text%20Len%20Dist.png" width: 500px; height: 400px; object-fit: cover;>

<h2>Key Insights</h2>
<ul>
  <li>The dataset is well-balanced across categories</li>
  <li>Combining title and description improves model performance</li>
  <li>TF-IDF effectively captures distinguishing textual features</li>
  <li>Logistic Regression performs well for multi-class classification</li>
</ul>

<h2>Prediction System</h2>
<p>A prediction system was implemented to classify new input text into one of the predefined categories.</p>
<p>The process involves:</p>
<ul>
  <li>Cleaning the input text using the same preprocessing steps</li>
  <li>Transforming the text using the trained TF-IDF vectorizer</li>
  <li>Passing the transformed data into the trained model</li>
  <li>Returning the predicted category label</li>
</ul>

<h3>Sample Input and Output</h3>
<p>Input: Team wins championship after thrilling final match <br>
Output: Sports</p>

<h2>Conclusion</h2>
<p>This project demonstrates how machine learning and NLP techniques can be used to classify textual data into multiple categories. 
It highlights the complete pipeline from preprocessing and feature extraction to model evaluation and prediction.</p>
