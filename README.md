# Real-time Twitter Sentiment Analysis for Topic Tracking

## Inspiration
The solution for evaluating Twitter data to perform better business decisions is to keep tracking all relevant Twitter content about a brand in real-time, perform analysis as topics or issues emerge, and detect anomaly with alert. By monitoring brand mentions on Twitter, brands could inform enagement and deliver better experiences for their customers across the world.

## Sample Output Plot

<img src="https://github.com/Chulong-Li/Twitter-Data-Sentiment-Analysis/blob/master/Figures/Complex.png" alt="Complex Dashboard" width="70%" height="70%">

## Get Started

### Pre-installation
```
pip install -r requirements.txt
```
### Set-up
Create a file called ```credentials.py``` and fill in the following content
```
# Go to http://apps.twitter.com and create an app.
# The consumer key and secret will be generated for you
API_KEY = "XXXXXXXXXXXXXX"
API_SECRET_KEY = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"

# After the step above, you will be redirected to your app's page.
# Create an access token under the the "Your access token" section
ACCESS_TOEKN = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
ACCESS_TOKEN_SECRET = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
```

Create local MySQL database with info below
```
host="localhost"
user="root"
passwd="password"
database_table="TwitterDB"
```

### Track Word Setting (Optional)
You can change the ```TRACK_WORDS``` in ```settings.py``` into any word, brand, or topic you're interested.


### Run
Run ```Main.ipynb``` to start scraping data on Jupter Notebook. 

Run ```live_sentiment-analysis.ipynb``` to perform data analysis for brand improvement after ```Main.ipynb``` starts running.

Note: Since streaming process is always on, press STOP button to finsih.
