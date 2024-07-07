# Epoch Core selection tasks

## Task 1 --- Classification Model

### Overview    

This task involves classifying data points using the K-means clustering algorithm. The objective is to identify distinct clusters within the data and determine the optimal number of clusters (K) using the elbow method.


#### Methods used:

#### a. K means clustering    
   An unsupervised machine learning algorithm used to partition the data into K clusters.
   
#### b. L2 norm for cluster distances   
  Used to calculate the Euclidean distance between data points and cluster centroids to minimize the within-cluster variance.
  
#### c. Elbow method to find the best K of clusters  
  A technique to determine the optimal number of clusters by plotting the sum of squared distances (inertia) and identifying the "elbow" point where the rate of decrease sharply slows.

#### Inferences :

a. The data for Maharashtra was in between some longitude and latitude hence made the data points in those lines.   
b. Implementation for L2 norm was new for me which I found for regularization of data    
c. The area near western ghats have less population density and hence the clusters there are sparse     
d. Also the nakshal region is sparsly populated   
e. Used geopandas for plotting India map   
f. optimal cluster =35-37

 ### Refrences :

 a. https://scikit-learn.org/stable/     

## Task 2 --- Sentiment Analysis of Handwritten Text Using Custom-built OCR and Sentiment Classification Models      

#### Methods used:   

a. CNN for training the model on alphabets    
b. Sliding window algorithm (lower version of YOLO) to segment the image into parts so as to predict each and every word     
c. Added an if statement for adding blank spaces as it was predicting a letter instead of blank space.
c. Pipeline -pipeline is a sequence of data processing and modeling steps, where each step transforms the data and passes it to the next step.       
    1. TfidfVectorizer transforms the text data into a numerical feature matrix where each row represents a document and each column represents a term, with the cell values being the TF-IDF scores.       
    2. Logistic regression model using the feature matrix to learn the relationship between the features (TF-IDF scores of terms) and the target labels (e.g., sentiments, categories).      
d. Sentiment Analysis     

#### Inferences :   

#### a. CNN is accurately predicting the alphabets       
#### b. The image segmentation accuracy is 100%     
#### c. Sentiment analysis accuracy      
  Achieved 66.67% accuracy on the validation set.    
  Achieved 88.33% accuracy on the test set.    

### Refrences:

a. https://www.youtube.com/watch?v=AsNTP8Kwu80  
b. https://www.youtube.com/watch?v=YCzL96nL7j0&list=TLPQMDcwNzIwMjQN9nIjk6PKMA&index=2
c. https://www.youtube.com/watch?v=HXjR2wDOfdA   ---- TfidfVectorizer + logistic regression in pipeline
