Should I pretend to love, or just like, this wine from Portugal?
========================================================
author: Catherine Pargeter
date: September, 2014
font-family: 'Helvetica'

Why Fake it?
========================================================

How many times have you been out with friends and "Know-it-All" Joe asks "Can you taste the hints of Alaskan salmon with a touch of of parsnip in that wine?", or you go to a wine tasting with a certain someone you want to impress and don't know what to think of the wines?

No body likes to look like a fool, so here is a way to fake your way through these awkward conversations.  

All you need is a quick chemical analysis of the wine, or use the information on the bottle along with the preset median values.  Use the sliders to enter the values, and get a prediction of whether the wine is terrible, pretty ok, or the best wine you have ever drank!

Check it out <a href = "https://cpargeter.shinyapps.io/Project/">here</a> next time you need to impress

How it works
========================================================
right: 68%
Using data from red and white wine from Portugal, the model takes the following characteristics into account:

  - fixed.acidity
  - volatile.acidity
  - citric.acid
  - residual.sugar
  - chlorides
  - free.sulfur.dioxide
  
  ***

Data from:  P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis. Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009. Via UCI Machine Learning Repository 
 - total.sulfur.dioxide
 - density
 - pH
 - sulphates
 - alcohol


Red Wine Model Accuracy, Specificity and Sensitivity
========================================================


```
[1] "Red Wine Accuracy: 0.8622"
```

```
       Sensitivity Specificity
Poor       0.05882      0.9978
Medium     0.96222      0.3780
Good       0.46154      0.9662
```



```
          Reference
Prediction   0   1   2
         0   1   1   0
         1  16 382  35
         2   0  14  30
```

White Wine Model Accuracy, Specificity and Sensitivity
========================================================


```
[1] "White Wine Accuracy: 0.8387"
```

```
       Sensitivity Specificity
Poor        0.1091      0.9958
Medium      0.9535      0.5013
Good        0.5692      0.9609
```


```
          Reference
Prediction    0    1    2
         0    6    6    0
         1   49 1045  137
         2    0   45  181
```
