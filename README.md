# How-to-create-reports-with-R-Markdown-in-RStudio

## Subscribe this YouTube Channel Data/Fun

#load required libraries
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

