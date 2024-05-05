# Correlation Bootstraps

In this assignment we explore the creation of the correlation statistic, which should be somewhat familiar from previous statistical
classes. We'll build this statistics by hand and use bootstrap
standard errors to estimate uncertainty around the statistic. 

When you submit your work, make sure to "knit" your RMD to an `.html` file and include that file in the repo you submit. (You can also knit to PDF and Word formats, which are great, but the HTML files are a bit easier for me to evaluate.) 

## Feedback 

In the first section, you write this
> I would expect the correlation coefficient to be furthest from zero when the proportion of observations with above average values in both variables is closest to 0.50. With this logic, I expect the coefficient for sustainability and localism to be greater than progressivism and age, and sustainability and progressivism.
>

Everything is perfect, except for the "0.5" inclusion. For instance, if we had two variables where this fraction was 0.7 or something, we'd have even higher correlations. (I guess this would require some pretty weird distributions, however.) 

You write
> #Can we be 100% confident the correlation is not 0? The odds of the true correlation coefficient being exactly zero seems nearly impossible.
>
True, it is nearly impossible. When we're talking about continuous random variables (like correlation), we typically don't talk about exact equality, since continuous variables, with their theoretically infinite precision, are never exactly equal to each other. Instead we talk about probability within some range of X values, just as you've done when you compare the replicates to the range from negative infinity to zero (`mean(result$statistic < 0)`). That's exactly the right way to think about it.

Excellent work on this. 
