# tomorrow
This demonstration website of the proof of concept based on a flask-web application is made by Dries de Roover, Michael Osuntuyi and Marya Dukmak.
This is a short explanation on how the proof of concept works. Make sure you have python 3 succesfully installed.
1. Firstly, install the requirements.text via pip/python3 to install all the dependencies;
2. Then run app.py and click on the link provided in the console;
3. You're all set. The system is now running locally on your PC.
When you want to have it running on a server, follow the same steps but add the following:
- Use a Screen like library on your linux system before running app.py;
- The application should then be still running on the server after you closed the command line window.

PLEASE NOTE that this proof of concept only contains Part B of the software. So it needs a pre-analysed data set of video/image/text data turned into a set of detected labels, objects and logos into a string in a CSV file. In short term, the video data is literaly text and the system compares text vs. text.
Part A is a data set of videos (or basicly every digital media) analysed using object, label and logo detection resulting into a CSV document. (latest.csv)

Functions:
- Sentiment analysis enables a review from very positive to very negative of both the article and the advertisement. When the article has a very bad sentiment no ad is being placed.
- Keyword analysis returns a list of the most important keywords using a fixed number of words. Both from the article as form the ad
- Similarity analysis returns a percentage of how similar the article and the ad are in text.

Possible updates and advise:
- A wider set of videos in the 'latest.csv' so that there is a broader range of advertisement possibilities.
- Text or image banners; at this moment the system only uses video's (youtube urls) to display ads. But in short the system only looks at the text from the article/website and the text data from a video. So if only text is provided it could still work.
- Turning the advertisement selection into an API.
  -   This allows the system to only analyse the text ONCE in stead of everytime. Now the matching process only works upon user request and needs to load every time.
  -   This decreases loading time and is more resource efficient.
  -   This API needs to be able to scrape the websites of where the ad would be placed.
