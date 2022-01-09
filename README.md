# NBA-Position-Prediction

### Hypotheses:
    It will be easiest to predict center and point guards because they are typically at the extremes of height, wingspan, rebounding, and assists
    Height, Wingspan, TRB%, AST%, STL%, and BLK% will be the best indicators of position

### Findings
One surprising finding in feature selection was the usefulness of Usage Percentage in classifying position. It is possible that Centers and Power Forwards might generally have lower Usage Percentage because they are more likely to be in the game for defensive purposes than smaller players. Regardless, I did not anticipate USG% being more important than a stat like Total Rebound Percentage because players playing the 3, 4, or 5 tend to grab more rebounds than guards.

The most accurate position classifier turned out to be the Decision Tree Classifier, although moving forward I would not recommend it as the best model to use for future NBA rosters. This is to say that I am not confident that the model as it is currently trained would perform as well on a larger sample size because it likely drew decision barriers that might not conform to future rosters. The nature of the NBA is changing by the moment as in some cases teams use much smaller centers in the interest of offensive versatilty and three point defense. The number of jumbo guards is also rapidly increasing with younger bigs learning to cater their games towards transition playmaking instead of inefficient low post scoring. My conclusion is that the GaussianNB model is the best model as it was the second most accurate and the underlying conditional probability would not suffer from the arbitrary lines in the sand that were drawn to optimize the prediction for about 700 data points with the Decision Tree Classifier would.
