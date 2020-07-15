# SBSPS-Challenge-1505-Sentiment-Analysis-of-COVID-19-Tweets-Dashboard-For-Visualization

# Overview: -
We choose to build a web app for analysis of people’s sentiments during lockdown in India.Our web app would provide proper sentiments analysis of peoples during lockdown with having relevant graphs, tables, and plots all of this is further compiled into a attractive user interactive web app. We also provide plots for all kinds of states in India for better analysis of peoples in different region. Not just stuck with only one kind of plot rather we provide different plots for some data.


# Purpose: - 
The problem statement that we choose to work on is to analyze sentiments of people during the epidemic so keeping this thought in our mind and making the web app according to it that is mainly focused to analyze sentiments of people from their texts extracted from twitter. Here the main purpose of the app is to give better insights of people sentiments during lockdown and predicting it further if lockdown extends. 

# The Problem Statement:-
According to the problem statement we have to analiyze sentiments of Indians before, after and during  the extension of lockdown announcements were made with the help of tweets on tweeter. We have to use relevant hashtags on twitter like #Lockdown, #COVID-19, #Coronavirus and build a predictive analytic model to understand the behavior of people towards the government decision and related schemes. We have to build a web app or dashboard for the visualization of people reaction towards the govt announcements on lockdown extension and related information

#  Proposed solution  :-  
After understanding all the problems and also finding a proper architecture for our web app we move to our solution part which is the start point of our whole application. For this firstly we collected tweeter data. For this there were two methods as disscussed in existing problem part. We choosed the second method that was collecting data from a website. For this firstly we downloaded the tweet id data of relevant dates ,i.e., from starting of first phase of lockdown till the fourth phase of lockdown for model training purpose and data of after that dates for prediction purpose. After the we used Hydrator app which automatically sets the twitter api rate limit and downloads the tweeter data in json format for the tweets id we provided. After that we converted that json data in csv file with the relevant tweeter data like date of tweet, tweet text, the sentiment vlaue and location of tweet. After that we filtered our data more deeply by sepecifing location that is India. After that we got the data for all phases of lockdown in India. After that we started model training. We used different models for training our model like Textblob, NLP, Bert. After that we checked accuracy and the model which gave the highest accuracy was selected. After that we moved to our next part which is web app building which will be a dashboard for visualization of sentiment analysis.For this first we started building the flask app which is a micro framework in python for doing the backend work of the web app. After that we started building the home page which consisted of sentiment values of tweets from all over of india. After that we built a map displaying the sentiment valueof different states with interactive features. After that we added some more interactivity on map ,i.e, added more information for each state so that if one clicks on a particular state on a map it redirects to a new page which shows a deeper analysis of that particular state. After that we added another template which displays the sentiment analysis of the indian tweets data on the bases of the four phases of the lockdown.For displaying the map on the home page and the page that displayes the state data we used Leaflet API , and also mapbox. For this we used mapbox to display basic map and after that we used leaflet to add interactivity to the map. For the analysis of tweets on each page we have dispalyed bar and line graphs with the help of  Plotly API in python. After that we made the prediction page where we are fetching the live tweet data from twitter using Tweepy api. And also we are analyzing the tweet entered by user to add more interactivity in our website. Also by this a user can understand that how accurately our model is predicting the sentiments of the tweets. Also this page shows prediction of future sentiments in line graph form which is also in plotly. Which helps one to understand that what will be the future prediction of the sentiments of the indian people towards lockdown and Government decisions related to covid-19.


# Result :---  
After that we completed all the mentioned above work , We are almost done. We till now completed model training, web app building and future prediction. As of now we have used different things like flask app, textblob, js library leaflet for map , plotly for graph and many other libraries. After that we have joined all the different components of our webpage ,i.e., we have linked all of our webpages together by a navigation bar. So till that pint our website is completed with al the backend , frontend and other inrteractive parts. After that we checked our website for working without any error. So as of now our work was done. So we deployed our whole website on IBM cloud using IBM cloud CLI. For this we deployed it with procfile, the manifest.yml file and also the requirement.txt file. So as of now our website is deployed. The link of our website is :-  http://covid19sentimentanalyzer-silly-buffalo-si.eu-gb.mybluemix.net/             

# Applications :-
 1. Our web app helps user to understand what people think about lockdown and what are their sentiments and behaviour towards lockdown. It helps user to understand wether people are happy or angry with the government decision related to lockdown. 
2. Our web app helps user to understand and comapre how people sentiments changed during different phase of lockdown. That is how people reactions changed during lockdown in all the diferent phases.
3. Our web app helps user to understand how the sentiments vaary from one state to another. That is how the sentiments of people changed during lockdown from one region to another. One can understand that what were the main reasons that is the main hashtags prevailing in one region and that were not in some another region.
4. Our webapp also helps one to analyize our model power by looking onto the prediction page where our powerful machine learning model works behind and helps user to understand that how in future the sentiments will prevail and what would be the major factors. Also there one can understand  whats the current scenario as we are fetching live tweets in table formation. Also there one can check our models accuracy as one can enter his tweets and check the sentiments towards that tweet and can understand how our model analysises text from different tweets.


# Conclusion :-
As aconclusion we have made a website which is deployed on this route :- http://covid19sentimentanalyzer-silly-buffalo-si.eu-gb.mybluemix.net/     . So as we can see from this website. We have done evrything as of now which was possible for doing sentiment analysis. So After viewing all the results and outputs from our website we can see that the number of positive and neutral tweets were in much larger amount as compared to negative tweets. Also tweets from first phase of lockdown are much more then any other phases of lockdown. We also see that as each phase passes by people tweeted less towards lockdown. Also from state wise analysis we see that the tweets realted towards lockdown were more from northern region as compared to eastern region. And all these anlaysis matched  the actual analysis from conditions around us. 
