# Assignment-2-Data-Bias
This project consists of the analysis of the Perspective API. Data_Bias_A2.ipynb notebook contains the code and markdowns that formulate my analysis.
The template and pre-labeled dataset contains a template for querying the Perspective API and the dataset that contains scores of comments as well as labels attributed to the comments; which were provided by the class for this assignment.

Exploration of the labeled dataset was done before the post test analysis which consisted of finding any correlation between the scores and the labels, parsing toxic words, and visualizing trends with boxplots.

The hypothesis was that the API determines the score based off of how many toxic words are condensed into the comment relative to the length of the comment and that casing of the comment can lead to a misleading score.

In conclusion, after conducting a linear regression test and querying specific words to test the case sensitivity of the API, I discovered that based off the linear regression test, there is a correlation between the length of the comment and the toxicity rating. Although there are many outliers, the RMSE somewhat proves that the Perspective API has a tendency to overlook the toxicity of a comment based on the length of the comment. By querying words with the class template, I discovered that casing matters for the perspective API as the example shows that 'penis' is rated .897 whereas 'PENis', which is the same word with different casing has an alarmingly lower rating of .168.
