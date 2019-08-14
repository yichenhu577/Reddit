### Problem Statement

As an employee of Niantic, the company behind the Pokemon Go mobile game, I'm interested in determing if there is a difference in post topics/contents between two Pokemon Go related subreddits (r/pokemongo and r/theSilphRoad). The r/pokemongo subreddit is supposedly tailored towards general topics of conversation while the r/theSilphRoad subreddit is supposedly more for research into the mechanics behind the game.

To determine if there is a difference, I will be using an number of classification models to predict whether a post belongs to r/theSilphRoad or not. I will be evaluating the models based on accuracy score and the coefficients of the model with the highest accuracy will be analyzed to determine what words/phrases are predictive of the specific subreddit.

Knowing this information is helpful since both of these subreddits contain end-user feedback regarding our game. Specifically, we would like to have our employees montoring these subreddits and if would be helpful to know if we should have employees monitoring both subreddits if the topics are roughly the same or if it would be best to assign a more technical employee to theSilphRoad subreddit.

### Notebooks / Process

#### Reddit Scraping

This notebook contains the code I used to scrape reddit over three consecutive days, aggregate the posts and remove duplicates

#### Processing

This notebook contains much of the processing (NLP and other) of the data obtained from my reddit scraping as well as some analysis of the differences between the subreddits

#### Modeling

This notebook contains the different models I tested as well as the analysis of the results of my best model

### Conclusions

It does seem like my model is able to predict between the two subreddits with my best model giving me a 21% increase in accuracy over the baseline model. However, it doesn't seem like most of my highest correlated words with theSilphRoad subreddit show the supposed research-heavy focus of the subreddit. This could either be because my model isn't great or because the subreddit itself doesn't actually focus as highly on research as it indicates. In any case, based on this analysis and the words that my model says are most predictive, I'm not seeing much reason from this analysis to dedicate a more technical employee to following theSilphRoad subreddit.