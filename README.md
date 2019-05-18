# How-to-create-reports-with-R-Markdown-in-RStudio
Data Science updates:-How to create reports with R Markdown in RStudio

# Subscribe to the YouTube channel for more videos in this series :-
https://www.youtube.com/channel/UCC5o...
.
# Follow us on FaceBook Link:-
https://www.facebook.com/Sckadam91
. 
# Instagram :- pythonrprogramming
.
Github link:-https://github.com/sujitkadam91/
## Subscribe this YouTube Channel Data/Fun

Below are sample R code

# load required libraries

install.packages(titanic)
library(titanic)
library(ggplot2)


# Data loading

df<-titanic_train
head(df)



# check data frame details


str(df)


# check summary of data frame 


summary(df)



# Bar plot -analysis of pclass with gender

ggplot(df, aes(x = Pclass)) + 
  geom_bar() + 
  facet_wrap(~Sex)


#### Subscribe this YouTube Channel Data/Fun
# Histogram -analysis of age with gender

ggplot(df, aes(x = Age)) + 
  geom_histogram() + 
  facet_wrap(~Sex)



# Density plot -Analysis of age with passenger class(pclass)

ggplot(df, aes(x = Age, fill = as.factor(Pclass))) +
  geom_density(alpha = .5)


# Thanks please subscribe my youtube channal Data/Fun

