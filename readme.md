# Twitter Sentiment Analysis with Spark Streaming

What we have is here a web application that takes an input keyword and loads the most recent tweets posted on Twitter with the keyword in them. The pulling of tweets is made possible by the use of the TweePy module, Spark Streaming and the [Twitter API](https://developer.twitter.com/en/docs/twitter-api). In order to use Twitter API, you need to sign up for a developer account on the given link. 

Once the tweets are loaded, they are put through Recurrent Neural Networks which predict whether the contents of the said tweet are positive or negative and a potential score of relaxed or tensed tone. Tweets in only English language are sourced using the filter function of the Stream. In addition to displaying the tweets, one can also view the distribution of sentiments with bar graph and pie chart. The most recurring words in the given tweets can be viewed with the word cloud. Plus, if the location of the tweet is available, they can be displayed on the world map. 

The Deep Learning models have been built with TensorFlow on the tweetsSample dataset, available in the repository. The app has to run a StreamListener in parallel with the main function and this is made possible using threading.

As the fetching of the tweets can take a minute, a progress bar displays upon entering the keyword:

<p align="center"><img src="https://user-images.githubusercontent.com/78029712/165440888-dbf25a23-6419-45d5-89f8-f9fa3b82947c.png" alt="drawing" width="600"/></p>

The loaded tweets screen appears like this:

<p align="center"><img src="https://user-images.githubusercontent.com/78029712/165441847-134da69a-ee6d-4ec5-927c-cbee3946b1f8.png" alt="drawing" width="600"/></p>

Once the tweets are loaded, you can choose from the visualisation options to see the distribution such as the pie chart below.

<p align="center"><img src="https://user-images.githubusercontent.com/78029712/165441418-91e87f33-70f2-4562-a201-23df5c67e68d.png" alt="drawing" width="600"/></p>

<p align="center"><b>Made with Python and Persistence</b></p>

**NOTE** - The Twitter Developer credentials have been removed due to privacy concerns. However, you can enter your own credentials and run this program. In order to run this program, you'd need to download this repository and enter the following command:

> python app.py

