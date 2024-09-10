# Foretelling The Stock Price Behavior Prediction By Top Twenty News Headlines Using Deep Learning & NLP
<p align="center">
<a href="https://nbviewer.jupyter.org/github/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Notebook/stock_price_behavior_prediction%20%282%29.ipynb" target="_blank">
  <img align="center"  src="https://github.com/NavinBondade/Distinguishing-Fake-And-Real-News-With-Deep-Learning/blob/main/Graphs/button_if-github-fails-to-load-the-notebook-click-here%20(4).png?raw=true"/>
</a>
</p>
<img src="https://www.thestreet.com/.image/t_share/MTcwMDkyODc4NDY5NTM5MTAy/stock-price-lead.jpg" alt="Fake_And_Real_News_Classification" width="970" height="510">
<p>News headlines play a crucial role in influencing stock price movements, as many investors base their trading decisions on the latest information. The sentiment expressed in these headlines—whether positive, negative, or neutral—directly affects the perception of a company's future performance, thereby impacting its stock price. Recognizing this, I have developed an advanced deep learning system that analyzes the sentiment of the top twenty news headlines related to a specific company to predict how its stock is likely to behave. By evaluating the emotional tone of the news, the system provides insights into whether a stock will rise, fall, or remain stable, offering valuable guidance to investors.

The deep learning system leverages Natural Language Processing (NLP) to understand and process news sentiment effectively. Trained on a vast dataset of historical stock prices and corresponding news articles, the model identifies complex patterns and relationships between headline sentiment and stock price movements. This predictive capability allows investors to anticipate market shifts with greater accuracy, helping them make more informed decisions. By providing a more comprehensive view of how external news events shape stock prices, this system empowers investors to adopt a more strategic and data-driven approach to trading.</p>
<h2>Libraries Used</h2>
<ul>
  <li>Tensorflow</li>
  <li>Keras</li>
  <li>Numpy</li>
  <li>Pandas </li>
  <li>Matplotlib</li>
  <li>Seaborn</li>
  <li>Sklearn</li>
  <li>Spacy</li>
  <li>BeautifulSoup</li>
  <li>Wordcloud</li>
</ul>
<h2>Target Class Distribution</h2>
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20%26%20Pictures/Distribution%20Of%20Dependent%20Variable.png">
<br>
<p align="center"> 
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20%26%20Pictures/Distribution%20Of%20Dependent%20Variable%20In%20Percentage.png">
</p>    
<h2>Model Details</h2>
<h2>Model Details</h2>
<p align="center">
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20&%20Pictures/model.png" alt="model" >
</p>
<p>
To predict stock price behavior based on the top twenty news headlines, I have developed a deep learning model composed of two distinct sections. The first section employs two one-dimensional convolutional layers, each followed by a max-pooling layer and a dropout layer. The convolutional layers are designed to capture the most relevant features and patterns from the input text, allowing the model to recognize important sentiment cues across the news headlines. The max-pooling layers help reduce the dimensionality of the data, preserving essential information while minimizing computational complexity. The dropout layers are incorporated to prevent overfitting, enhancing the model’s generalization capability by randomly deactivating a subset of neurons during training.

The second section of the model consists of three fully connected dense neural network layers, which further process the extracted features and refine the predictions. Each dense layer uses the Rectified Linear Unit (ReLU) activation function, ensuring the model can learn complex, non-linear relationships in the data. The final dense layer, however, utilizes a sigmoid activation function to map the output to a probability range between 0 and 1. This allows the model to effectively predict the likelihood of a stock price increasing or decreasing, based on the sentiment extracted from the headlines. By combining convolutional layers for feature extraction with dense layers for decision-making, the model is able to deliver highly accurate predictions of stock price movements.</p>
<h2>Model Traning</h2>
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20%26%20Pictures/loss-accuracy.png" alt="loss_accuracy">
<p>The model was trained over the course of five epochs, utilizing the Adam optimizer to ensure efficient and adaptive learning. Adam is particularly well-suited for this type of task due to its ability to handle sparse gradients and adjust learning rates dynamically, allowing for faster convergence. The loss function employed during training was mean squared error (MSE), which was chosen to penalize the model more heavily for incorrect predictions. By minimizing the squared differences between predicted and actual values, MSE ensures that the model learns to make more accurate predictions while reducing the impact of larger errors.

Upon completion of training, the model demonstrated impressive performance on the training data, achieving a high accuracy of 98%. Additionally, the training loss was minimized to a low value of 0.014, indicating that the model is not only highly accurate but also well-calibrated, with minimal prediction error. These results suggest that the model has successfully learned to generalize from the data and is capable of making precise predictions, further solidifying its effectiveness in forecasting stock price movements based on news headlines.</p>

<h2>Model Evaluation on Development Dataset</h2>
<ul>
  <li><b>Training Data Accuracy: 98%</b></li>
  <li><b>Training Data Loss: 0.014</b></li> 
  <li><b>Test Data Accuracy: 99%</b></li>
  <li><b>Test Data Loss: 0.026</b></li> 
</ul>
<br>
<h2>Confusion Matrix</h2>
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20%26%20Pictures/Confusion%20Matrix.png" 
     style="display: block; margin-left: auto; margin-right: auto;">

<h2>Classification Report on Development Dataset</h2>
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20%26%20Pictures/Classification%20Report.png" 
     style="display: block; margin-left: auto; margin-right: auto;">

<h2>Conclusion</h2>
<p>In this project, I have created a deep learning model that foretells how the stock price of a company will behave by considering major news headlines with an impressive accuracy of 98 percent.</p>
