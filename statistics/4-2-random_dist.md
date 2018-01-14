[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

x = pd.DataFrame(np.random.random(1000), columns= ["rand"])

dfg = x.groupby("rand").nunique() / x.count()#.reset_index()
dfg.columns.values[0] = 'count'
dfg["rand"] = dfg.index

fig, ax = plt.subplots()
ax.bar(dfg["rand"], dfg["count"], width= 0.001, linewidth= 0,edgecolor ="red", align  = 'center')  
```
![pdf](https://github.com/lh209/dsp/blob/master/img/4_1.png)


```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

x = pd.DataFrame(np.random.random(1000), columns= ["rand"])

dfg = x.groupby("rand").nunique() 
dfg.columns.values[0] = 'count'
dfg["rand"] = dfg.index
dfg['cdf'] = np.cumsum(dfg["count"])/ x.count()[0]

plt.scatter(dfg["rand"], dfg['cdf'], s=.5)
```

![cdf](https://github.com/lh209/dsp/blob/master/img/4_2.png)

>> yes
