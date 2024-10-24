# Kickstarter_ML_project
In the past decade, the number of ways small companies and individuals can fund their projects has grown considerably. In addition to savings, bank loans, friend and family funding, crowdfunding has grown in popularity. The crowdfunding platform, Kickstarter, was created in 2009 and has an all or nothing funding model. This means that a project is only funded if it reaches its goal amount; otherwise no money is given by the backers of the project. 

A wide variety of factors contribute to the success or failure of a project, both in general and on Kickstarter. Some of these factors can be quantified, which allows for the creation of a model that can predict whether a project will fail or succeed. The aim of this project is to construct such a model and analyze Kickstarter data, in order to assist potential content creators to assess whether Kickstarter will be a viable funding option for them and what their chances of success are.

The dataset used in this project was downloaded as .csv file from a webscrape done by a webscraping site Web Robots. This dataset contains information about projects hosted on Kickstarter from April 2009 to late 2019.

# Final Results
Each model was able to achieve an accuracy of between 70%-74% after parameter tuning. Although it was easy to achieve an accuracy of 70%, after parameter tuning the accuracy only increased by a small amount. It is possible that the large amount of data only in two categories meant that there was enough data to perform a simple model (like basic logistic regression). <br>

The final model choosen was the Random Forest model with an F1 score of 0.744. <br>

Interestingly, each model performed did not do a good job of predicting failures compared to successful projects, with a lower true negative than true positive rate. It is likely that things that cause projects to fail are outside the scope of the given data, eg. poor marketing, insufficient updates or not not replying to potential backers.

# Recommendations
Some of the featues had a positive effect on the sucess rate and/or the amount of money received (as deduced by feature importance and feature engineering): <br>

Most Important: <br>
1. Smaller project goals <br>
2. Being choosen as a staff pick <br>
3. Shorter campaigns <br>
4. Longer campaign to launch duration <br>
5. Comics, dance and games projects <br>

Least Important: <br>
1. Projects from Hong Kong <br>
2. Launching a project on a Tuesday (this is the most popular day to launch a project, so beware competition) <br>
3. Name length and blurb length (shorter blurbs and longer names are preferred) <br>
4. Film and music projects are most popular categories on site and are fairly successful <br>
5. Launching a campaign between 12pm and 2pm UTC (related to country of origin) <br>

The factors that had the most negative effect on success rate and/or the amount of money receieved are: <br>

Most Important: <br>
1. Larger goals <br>
2. Longer campaigns <br>
3. Food and journalism projects <br>
4. Projects from Italy <br>

Least Important: <br>
1. Launching on the weekend <br>
2. Launching in July or December <br>
3. Launching between 4am and 6am UTC <br>

Overall, Kickstarter is well-suited for smaller, high quality projects(particularly comics, dances and games) and less-suited to larger projects like journalism and food projects.
