CHAPTER 7: THE NORMAL PROBABILITY DISTRIBUTION

- 7.1 Properties of the Normal Distribution
  - (1) Use the uniform probability distribution
    - When two intervals of equal length are equally likely, the random variable X is said to follow a **uniform probability distribution**
    - For continuous random variables, the probability of observing one *particular* value is zero
    - To resolve this problem we compute probabilities of continuous random variables over an *interval* of values using *probability density functions* (in contrast to the *probability distribution functions* used for discrete random variables)
    - A **probability density function (pdf)** is an equation used to compute probabilities of continuous random variables. It must satisfy the following two properties:
      - (1) The total area under the graph of the equation over all possible values of the random variable must equal 1. 
      - (2) The height of the graph of the equation must be greater than or equal to 0 for all possible values of the random variable.
    - The area under the graph of a density function over an interval represents the probability of observing a value of the random variable in that interval
  - (2) Graph a normal curve
    - In mathematics, a **model** is an equation, table, or graph used to describe reality
    - A continuous random variable is **normally distributed**, or has a **normal probability distribution**, if its relative frequency histogram has the shape of a normal curve
    - For symmetric distributions with a single peak, such as the normal distribution, the mean = median = mode
    - Because of this, the mean, mew, corresponds to the high point of the graph of the distribution
    - The points at x = mew - sigma and x = mew + sigma are the **inflection points** on the normal curve, the points on the curve where the curvature of the graph changes
  - (3) State the properties of the normal curve
    - **Properties of the Normal Density Curve**
      - (1) The normal curve is symmetric about its mean, mew.
      - (2) Because mean = median = mode, the normal curve has a single peak and the highest point occurs at x = mew.
      - (3) The normal curve has inflection points at mew - sigma and mew + sigma
      - (4) The are under the normal curve is 1
      - (5) The area under the normal curve to the right of mew equals the area under the curve to the left of mew, which equals 1 / 2.
      - (6) As x increases without bound (gets larger and larger), the graph approaches, but never reaches, the horizontal axis. As x decreases without bound (gets more and more negative), the graph approaches, but never reaches, the horizontal axis
      - (7) The Empirical Rule:
        - Approximately 68% of the area under the normal curve is between x = mew - sigma and x = mew + sigma
        - Approximately 95% of the area is between x = mew - 2(sigma) and x = mew + 2(sigma)
        - Approximately 99.7% of the area is between x = mew - 3(sigma) and x = mew + 3(sigma)
  - (4) Explain the role of area in the normal density function
    - The equation (or model) used to determine the probability of a continuous random variable is called a **probability density function** (or **pdf**)
    - The **normal probability density function** is given but the equation will not be used in this text
    - Instead, we will use the normal distribution in graphical form by drawing the normal curve
    - Area under a Normal Curve
      - Suppose that a random variable X is normally distributed with mean mew and standard deviation sigma. The area under the normal curve for any interval of values of the random variable X represents either
        - The proportion of the population with the characteristic described by the interval of values
        - The probability that a randomly selected individual from the population will have the characteristic described by the interval of values
- 7.2 Applications of the Normal Distribution
  - (1) Find and interpret the area under a normal curve
    - We have two options for finding the area under the normal curve-- by-hand calculations with the aid of a table or technology
    - We use z-scores to help find the area under a normal curve by hand
    - Standardizing a Normal Random Variable
      - Suppose that the random variable X is normally distributed with mean mew and standard deviation sigma. Then the random variable Z = (X - mew) / sigma is normally distributed with mean mew = 0 and standard deviation sigma = 1. The random variable Z is said to have the **standard normal distribution**.
    - This result is powerful! If a normal random variable X has mean different from 0 or a standard deviation different from 1, we can transform X into a **standard normal random variable Z** whose mean is 0 and standard deviation is 1. Then we can use Table V to find the area to the left of a specified z-score, which is also the area to the left of the value of x in the distribution of X. We are find the area under the **standard normal curve**.
    - In this text we round z-scores to two decimal places
    - Technology Approach:
      - **TI-84: Use the normalcdf function**
        - **normalcdf(lower bound, upper bound, mean, standard deviation)**
    - Summary of Methods for Obtaining the Area Under a Normal Curve
      - (1) Find the area to the left of x.
        - Convert the value of x to a z-score and use Table V to find the area to the left of z (and x).
        - OR use technology.
      - (2) Find the area to the right of x.
        - Convert the value of x to a z-score and use Table V to find the area to the left of z (and x). The area to the right of z (also x) is 1 minus the area to the left of z.
        - OR use technology.
      - (3) Find the area between x1 and x2.
        - Convert the values of x to z-scores and use Table V to find the area to the left of z1 and z2. The area between z1 and z2 is (area to the left of z2) - (area to the left of z1).
        - OR use technology.
    - Some Cautionary Thoughts
      - The normal curve extends indefinitely in both directions; for this reason, there is no range of values of a normal random variable for which the area under the curve is 1
      - If software reports an area as 1, we will follow the practice of reporting such areas as >0.9999
      - If software reports an area as 0, we will follow the practice of reporting such areas as <0.0001
  - (2) Find the value of a normal random variable
    - Often, we do not want to find the proportion, probability, or percentile given a value of a normal random variable
    - Rather, we want to find the value of a normal random variable that corresponds to a certain proportion, probability, or percentile
    - By-Hand Approach
      - Step 1) Draw a normal curve and shade the desired area
      - Step 2) Use Table V to find the z-score for the area that's closest to the shaded area
      - Step 3) Obtain the normal value from the formula x = mew + z(sigma)
    - Technology Approach
      - Step 1) Draw a normal curve and shade the desired area
      - Step 2) TI-84: **Use the function invNorm()**
        - **invNorm(area left, mean, standard deviation)**
- 7.3 Assessing Normality
  - (1) Use normal probability plots to assess normality
    - A **normal probability plot** is a graph that plots observed data versus *normal scores*
    - A **normal score** is the expected z-score of the data value, assuming that the distribution of the random variable is normal; the expected z-score of an observed value depends on the number of observations in the data set
    - Drawing a Normal Probability Plot
      - Step 1) Arrange the data in ascending order.
      - Step 2) Compute *fi*, where *i* is the index (the position of the data value in the ordered list) and *n* is the number of observations. The expected proportion of observations less than or equal to the *i*th data value is *fi*.
      - Step 3) Find the z-score corresponding to *fi* from Table V.
      - Step 4) Plot the observed values on the horizontal axis and the corrsponding expected z-scores on the vertical axis.
    - If sample data are taken from a population that is normally distributed, a normal probability plot of the observed values versus the expected z-scores will be approximately linear.
    - If the linear correlation coefficient between the observed values and expected z-scores is greater than the critical value found in Table VI, then it is reasonable to conclude that the data could come from a population that is normally distributed
- 7.4 The Normal Approximation to the Binomial Probability Distribution