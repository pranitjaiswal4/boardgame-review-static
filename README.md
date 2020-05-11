# Steps to deploy my text classifier model as a web application:   

---------------------------------------------------------------------------------------------------------------------------------
    
1. You can take dump of the Vectorizer and Best Classifier in the local files using the following code in notebook:   
(https://pranitjaiswal.netlify.com/files/Jaiswal_Project.ipynb)   
   
(Note: To avoid any possible errors, kindly don't change the following filenames)   
   
###### * Take dump of Best Classifier using Pickle   
pickle.dump(bestClassifier, open('model.pkl', 'wb'))   
   
###### * Take dump of Vectorizer using Pickle   
pickle.dump(tfidfconverter, open('tfidfconverter1.pkl', 'wb'))   
   
###### * Take extra dump of Vectorizer using Pickle (in case .pkl files are not supported in your flask app)   
pickle.dump(tfidfconverter, open('tfidfconverter2.pickle', 'wb'))   
   
- OR -   
   
You can also find these files in this repository:   
(https://github.com/pranitjaiswal4/rating-predictor-app)   
   
---------------------------------------------------------------------------------------------------------------------------------
   
2. Download the whole source code from this repository:   
(https://github.com/pranitjaiswal4/rating-predictor-app)   
   
---------------------------------------------------------------------------------------------------------------------------------
   
3. Open Terminal of the system where you wish to host/run this application   
   
---------------------------------------------------------------------------------------------------------------------------------

4. Go to the path of the directory in which you downloaded the source code   

---------------------------------------------------------------------------------------------------------------------------------
   
5. Steps to setup the web app run enviornment in Linux OS:   
(Note: Below steps may differ for different OS)   
   
a) Run below command to create python virtual environment   
-> python3 -m venv venv   
   
b) Run below command to initiate virtual environment   
-> source venv/bin/activate   
   
c) Install libraries using pip command   
-> pip install pickle flask numpy pandas sklearn   
   
d) Run the app:   
-> python3 app.py   
   
---------------------------------------------------------------------------------------------------------------------------------
