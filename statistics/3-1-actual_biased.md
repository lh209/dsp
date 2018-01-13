[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)


'''python
import matplotlib.pyplot as plt
kids = df.loc[:,"numkdhh"]
pmf = kids.value_counts().sort_index() / len(kids)
pmf.plot(kind='bar')
'''

![unbiased](https://github.com/lh209/dsp/blob/master/img/3_1.png)

'''python
import numpy as np 
kidsBiased = df[df.loc[:,"numkdhh"] > 0]["numkdhh"]
kids2 = np.repeat(kidsBiased,kidsBiased)
pmf = kids2.value_counts().sort_index() / len(kids)
pmf.plot(kind='bar')
'''

![unbiased](https://github.com/lh209/dsp/blob/master/img/3_2.png)