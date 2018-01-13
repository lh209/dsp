[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```python 
firstborn = live[live["pregordr"] == 1]["totalwgt_lb"]
restborn = live[live["pregordr"] > 1]["totalwgt_lb"]

CohenEffectSize(restborn,firstborn)
```

>> 0.069119360198852148
