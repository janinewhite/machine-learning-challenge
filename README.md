# machine-learning-challenge
 
This is an exploration of predicting exoplanets.I began by renaming the data analysis by renaming the variables so that I could understand what they meant, then I graphed each of them by whether they were confirmed as exoplanets or not.  I also ran logistics regressions on all of the primary variables, not the tolerances, to see the strength of the relationships with confirming an exoplanet. The training and testing scores for the logistic regressions were .74.

![Logistic Regression Coefficients](https://github.com/janinewhite/machine-learning-challenge/blob/master/logistic%20regression%20coefficients%20graph.png?raw=true)

I used the variables that showed some relationship with confirming an exoplanet to build a TensorFlow model. I tested various combination of epochs and nodes, including up to 200 epochs and 80 nodes.  I settled on 27 nodes and 15 epochs because increased epochs and nodes did not significantly increase the accuracy or reduce loss from 0.40 loss and .76 accuracy.

![Epochs](https://github.com/janinewhite/machine-learning-challenge/blob/master/epoch%20accuracy%20and%20loss.png?raw=true)

The slight increase in accuracy in TensorFlow would not encourage me to use that type of modeling over regression because it is far less understandable.  It does not easily provide an avenue for reducing data collection efforts or analysis complexity, which can lead to increased costs.
