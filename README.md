# Community Vitality in the Quad Cities

## Abstract
This project is meant to analyze the community vitality of the Quad Cities--a community in Iowa and Illinois--using local perspectives. To do this, I conducted Twitter sentiment analysis on local tweets using a natural languagae processing library. By analyzing the sentiment and polarity of these tweets and visualizing the results with word clouds, I was able to get a sense of the local perception of community vitality and areas for improvement.

## Methods
### Data Source
I selected local tweets that included the name of one of the Quad Cities and a word related to one of my five chosen categoris: crime, education, arts, and infrastructure. The Twitter API made this queries quite simple to pass through. I was able to write specific queries for each of the five categories to return tweets for analysis. For example, the crime tweets query would have selected tweets that included "Davenport" and "shooting" or "Moline" and "theft." These tweets are selected from the last week.

### Data Cleaning
The data cleaning step is mostly handled by the Twitter API. However, I did remove retweets, tweets not in English, and usernames (for the world cloud).

### Sentiment Analysis Tools
I mainly used the Python TextBlob library to perform the natural language processing (NLP). Per the TextBlob documentation, "TextBlob aims to provide access to common text-processing operations through a familiar interface. You can treat TextBlob objects as if they were Python strings that learned how to do Natural Language Processing." The most useful part of this library was the ability to categorize tweets by polarity (a negative number, positive number, or zero) and subsequently the sentiment (negative, positive, neutral).

### Creating Word Clouds
To visualize the results, I used the Word Cloud library in Python, which allowed me to generate word clouds from the tweets based on their frequency. The most common words appear largest, which adds to the visual representiation of local perceptions on my community.

### Reliability and Validity
Based on manual analysis of the tweets (i.e., looking at the tweets myself to see if they fit the category and the assigned sentiment), these methods seem to work well. However, this is not to say that it is perfect. For example, sentiment analysis is not as helpful for the crime category where most tweets are negative (but many have been assigned positive).

### Writing Functions
Below are several functions I wrote to extract, clean, and analyze data and create the world clouds. The comments above each function should give an adequate description of what it does.

## Takeaways
**Crime:** Public perception of crime centers on the police, whether positive or negative. Further, in just a week's worth of tweets the involvement of race in these discussions is clear. One Moline Police Department officer is frequently mentioned on their social media despite his lack of experience but likely because he is black. "Black" is also one of the most common words in the negative word cloud. In my own experience, black people in our community are arrested at much higher rates and community awareness of this is not very high--leading to further anti-black rhetoric.

**Education:** Education seems to center around sports, with "basketball" (the sport in season) and "championship" being relatively large. Currently contentious issues seem to be sex ed and the accessibility of porn online, leading to words like "sexual," "internet," "accessible." Religious terms also appear because of attempts to use immorality to justify exclusion of certain topics (of a sexual nature or in relation to banned books).

**Arts:** The arts category seems to have the most variety in general topic areas, which is what I would have expected. The Quad Cities have vibrant live music scenes as well as successful school music programs (there were several tweets about my high school's band going to London to perform at a New Year's parade).

**Infrastructure:** Infrastructure discussions, as expected, are mostly complaints or updates about roads, highways, and bridges. Specifically, a new bridge was just built and another is being planned (over the "Mississippi," another frequent term).

**Environment:** The largest word: snow. This is likely because a very large snow storm coming this week that will shut down much of the Quad Cities (in addition to -38 degree weather). Much of the other positive environmental discussions deal with forecasts, while negative sentiment applies to pollution in the Mississippi River (which is source of water).

Overall, my community seems to be focused on short-term. Even with tweets over the last week, very few reference anything outside of that. For example, the environment discussions center on current weather, infrastructure tweets deal with closures and updates on construction, etc. This focus on only the current week may be due to a variety of factors, but I attribute it mostly to financial constraints (and the lack of considering long term benefits that comes with financial instability). In my most immediate community, many families around me do not have the overall vitality necessary to consider their future happiness, instead they are just trying to survive. This mindset is seen clearly in the analysis of these tweets. My hope for the future of my community is that people of color will have more access to opportunity, allowing them to think outside of the present. This opportunity would help to create a more sustainable and thriving environment for all members of our community.
