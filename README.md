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
<p>For the prediction of the stock price behaviors with top twenty news headlines, I have created a deep learning model that is divided into two sections, the first section uses two one dimensional convolutional layers each followed by a max-pooling and dropout layer, and the second section uses three fully connected dense neural network layers. All the layers use RELU as an activation function except the last dense layer that uses the sigmoid activation function to map predicted values to probabilities between 0 and 1.</p>
<h2>Model Traning</h2>
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20%26%20Pictures/loss-accuracy.png" alt="loss_accuracy">
<p>The model has been trained for five epochs. During training, the model uses Adam as an optimizer. The loss function used was mean square error to penalize the model more whenever it makes false predictions.</p>

<h2>Model Evaluation on Development Dataset</h2>
<ul>
  <li><b>Training Data Accuracy: 98%</b></li>
  <li><b>Training Data Loss: 0.014</b></li> 
  <li><b>Test Data Accuracy: 99%</b></li>
  <li><b>Test Data Loss: 0.026</b></li> 
</ul>
<br>
<h2>Confusion Matrix</h2>
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20%26%20Pictures/Confusion%20Matrix.png">
<h2>Classification Report on Development Dataset</h2>
<img src="https://github.com/NavinBondade/Foretelling-The-Stock-Price-Behavior-With-Major-News-Headlines/blob/main/Graphs%20%26%20Pictures/Classification%20Report.png">   
<h2>Conclusion</h2>
<p>In this project, I have created a deep learning model that foretells how the stock price of a company will behave by considering major news headlines with an impressive accuracy of 98 percent.</p>
