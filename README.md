# Getting Started

The code demonstration explains how the bootstrap method works in the field of statistics.

## What is Bootstrapping?
Bootstrapping is a method that uses random sampling with replacement to estimate quantities about a population. As we draw samples, we will make statistical calculations (such as finding the mean, median, or variance) based on each simulated dataset and then find the mean of that statistic across all samples. These samples are constructed by drawing observations from our original dataset and returning them to the data sample after they have been chosen. Afterwards we will plot them to understand the shape of our data to make inferences about our entire population.

### Sampling with replacement
Sampling with replacement occurs when a unit is drawn from a finite population and is returned to that population, after its characteristic(s) have been recorded, before the next unit is drawn. Every time we draw an element from our dataset, we will record it on our simulated dataset (known as bootstrapped dataset) and return it to the population afterwards.

### Caveats
Although bootstrapping is a powerful technique, it has some limitations:
* It requires a considerable amount of computational power
* It requires a representative sample to be effective
* Simple bootstrapping may be misleading when the underlying distribution has fat tails

bootstrapping is still considered a very useful technique because it saves time and resources when collecting data to study the population, can be used with small datasets and handles outliers and influential points well.

### Applications to Machine Learning
When building machine learning models, we can use bootstrapping to simulate the dataset on which our model will be trained on. The quality of our model will then be accurately assessed against a portion of the original dataset that was not utilized to create the bootstrapped training set. Read more about it on [Wikipedia](https://en.wikipedia.org/wiki/Bootstrapping_(statistics)). 


![Bootstrapping Illustration](https://github.com/Lawrence-LUOoo/Bootstrapping-Code-Demonstration/blob/main/bootstrapping_illustration.jpeg) [Image Source](https://trisxcjoseph.medium.com/)

We usually gather samples from the original population to obtain a distribution and its statistics (illustrated in blue). Bootstrapping allows us to produce similar result but through a smaller sample size via resampling with replacement method (illustrated in yellow).

## Installation
Use the package manager [pip](https://pip.pypa.io/en/stable/) to install numpy and matplotlib.

```bash
pip install numpy
pip install matplotlib
pip install scipy
```

Execute the notebook [Bootstrapping - Code Demonstration.ipynb](https://github.com/Lawrence-LUOoo/Bootstrapping-Code-Demonstration/blob/main/Bootstrapping%20-%20Code%20Demonstration.ipynb) cell-by-cell to understand how each part of bootstrapping works.

Execute the notebook [r_squared_bootstrapping.ipynb](https://github.com/Lawrence-LUOoo/Bootstrapping-Code-Demonstration/blob/main/r_squared_bootstrapping.ipynb) cell-by-cell to understand how we can use bootstrapping to get an approximate sample distribution of R<sup>2</sup> for a simple linear regression model. 

## Analysis steps
1. Simulate population distribution
2. Take a random sample from the population
3. Bootstrap for 10,000 times
4. Analysis and interpretation
5. Plot the probability distribution and confidence interval

## Authors:
+ [Ruifeng Luo](https://github.com/Lawrence-LUOoo)
+ [Charudatta Manwatkar](https://github.com/CharudattaManwatkar)
+ [Siew Tsien (Hanna) Lee](https://link-url-here.org)
+ [Camilo Chaves Beltran](https://link-url-here.org)
