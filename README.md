# spotifyhitpredictor
What makes a song go "Viral"? Using this information, we can both advise new singers on how to increase virality as well as make our own music with more success.

In this project we set out to analyse the variables contributing to the success of any one song. We aim to build a model from data obtained via Spotify to predict the factors that will make a song successful in the future decade. We will also perform a decade-by-decade analysis of how our these variables trended over time.

The key questions we will answer are;

What variables matter most when it comes to a song’s success?
How have these variables “varied” over time? 😉
Can we predict the potential success of a new song?
If you were a singer or a production company, and you came to us, can we advise you?
We will be regressing a “target” variable which is binary in nature and takes the value of 1 if a song is a hit and 0 if a song is a flop (based on billboard hit list charts). Since this variable is binary, a simple linear regression is a poor fit (as illustrated in later sections) and thus we use a generalized linear model (glm) specifically, a logit model - a logistic regression.

In order to construct this regression, we will regress our target variable on a few important explanatory variables including Danceability, Energy, Key, among others. We will do this for 3 decades 1960-1970, 1990-2000, and 2010-2019. By eliminating insignificant variables for each model, we will then arrive at 3 optimized logistic regression models for each decade and we will intepret those results.

Finally, we will construct a prediction model using k-fold cross validation, and test the accuracy for each of our 3 models. We will illustrate this accuracy by also constructing confusion matrices, and ROC curves, and calculating the area under the ROC curves for each model.

In the end, due to high accuracy of our 2010-2019 model, we will recommend that model for future artists to improve their chances of success by improving variables like Danceability, which have been important throughout time, but also optimizing time siganture and loudness to create the perfect song.
