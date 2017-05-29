# Section 2
## Types of Data
- **Numerical**: represents some sort of quantitative measurement (heights, page load times, stock prices)
  - Discrete data is integer based; often counts of some event (purchases, coin flips)
  - Continuous data is based on an infinite number of possible values (time taken, amount of rainfall)

- **Categorical**: qualitative data that has no inherent mathematical meaning (gender, state of residence, product category)

- **Ordinal**: mixture of numerical and categorical data; where the variables have natural, ordered categories and the distances between the categories is not known (movie ratings on a 1-5 scale)

## Standard Deviation and Variance
Variance measures how "spread-out" the data is. It is the average of the squared differences from the mean. Squaring the differences from the mean amplifies the outliers in the data. Standard deviation is the square root of the variance and is used as a way to identify outliers. Data points that lie more than one standard deviation from the mean can be considered unusual.

If given a complete set of data/observations, population variance can be calculated normally. However, if taking a sample/subset of the data, you take the sample variance which is the average-1 of the squared differences from the mean.

## Probability Density and Mass Functions
The probability density function, given a range of values, defines the probability of landing within that range for a continuous random variable. The probability mass function is used for discrete data and is represented by a histogram rather than a continuous curve.

Uniform distribution is where every range of values has the same constant probability of occurring. Normal distribution is where the majority of values lie within 1-2 standard deviations from the mean. Exponential distribution has an exponential fall-off.

Binomial probability mass function is used when there are exactly two mutually exclusive outcomes of a trial and obtains the probability of observing the number of successes in a certain number of trials based on the formula. Poisson probability mass function is used to predict the probability of a given number of events occurring during some interval of time with a known average rate that is independent from the previous event.

## Percentiles and Moments
The interquartile range for a set of values contains 50% of the data distribution and is typically located near the mean. The 90th percentile represents the value where < 90% of the data is located on the distribution. Outliers bounds are defined as any data points that lie outside 1.5*IQR.

**Moments** are quantitative measures of the shape of a probability density function. The first moment is the mean, the second moment is the variance. The third moment is "**skew**" which is a measure of how "lopsided" the distribution is where a negative skew is when the data distribution has a longer tail on the left. The fourth moment is "**kurtosis**" which is a measure of the thickness of the tail and the sharpness of the peak compared to a normal distribution. Higher peaks have higher kurtosis values.

## Covariance and Correlation
Covariance measures how two variables vary in tandem from their means. To measure covariance, convert data sets for the two variables into vectors of variances from the mean with the dimension of the vector representing the length of the data set. Then, take the dot product (cosine of the angle between them) of the two vectors and divide by the sample size. If the covariance is close to 0, then there is little correlation between the two variables. A large covariance means there exists some correlation but how to identify significance?

Correlation is found by normalizing the covariance from -1 to 1 by dividing it by the standard deviation of both variables. A correlation of -1 means a perfect inverse correlation.

## Conditional Probability
P(B|A) = P(A,B) / P(A) is the probability of event B given that A has occurred. P(A,B) is the probability of event A and B both occurring. If event A and B were independent then P(B|A) should be about the same as P(B).

## Bayes' Theorem
P(A|B) = P(A) * P(B|A) / P(B). The key insight is that the probability of something that depends on B depends very much on the base probability of B and A. Drug testing and false positives is a common example where Bayes' Theorem applies. Even if P(B|A) is high, it doesn't mean that P(A|B) is also high. A high accuracy rate of a drug test can lead to misleading results if the incidence of the drug usage is low.
