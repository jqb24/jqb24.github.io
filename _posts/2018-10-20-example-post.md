---
layout: post
title: Example Post
date: 2017-09-12 00:00:00 +0300
description: Here is an example post # Add post description (optional)
img: how-to-start.jpg # Add image post (optional)
tags: [Programming, Learn] # add tag
use_math : true
---

Here is my first example blog post.

## Subtitle

``` python
#!/usr/bin/python
import quandl
import matplotlib.pyplot as plt

import pandas_datareader as pdr
import pandas as pd
import datetime
import statsmodels.api as sm

tickers = []

def get(tickers):
    def data(ticker):
        return (pdr.get_data_yahoo(ticker))
    datas = map(data, tickers)
    return (pd.concat(datas, keys=tickers, names=['Ticker'])

aapl = pdr.get_data_yahoo('AAPL')

#Rule 3 - Buy Stocks Above Their 200-day Moving Average,Not Below
adjClose = pd.DataFrame(aapl['Adj Close'], index = aapl.index)
adjClose['ma'] = adjClose.rolling(window=200).mean()


df=pd.DataFrame(np.random.randn(10,4), index=range(10), columns=list('ABCD'))

df['GROUP'].isin([2,5])
df[df>0]=1
df.dropna(how='any')
df.fillna(value=5)
pd.isnull(df)
df2=[df[:3],df[:5]]
pd.concat(df2)
right=pd.DataFrame({'firstname': ['Henry', 'Jones','Indiana'], 'location': [1, 2,3]})
people.groupby('gender').min()
df["grade"].cat.categories = ["very good", "good", "very bad"]
df.groupby("grade").min()
ts.resample('D')
ts.shift(2)
offset.rollforward(now)

###
def get(tickers):
    def data(ticker):
        return (pdf.get_data_yahoo)
datas = map(data, tickers)
return (pd.concat(datas, keys=tickers, names=['Ticker'])
```

## Next Subtitle
* Here
* is
* a list

### Numbered list
1. Here
2. is
3. a numbered
4. list

## LaTeX!!!
You can display equations as a block...
$$
\begin{bmatrix}
    \cos 90^{\circ} & \sin 90^{\circ}\\
   -\sin 90^{\circ} & \cos 90^{\circ}
\end{bmatrix}
\begin{bmatrix} a1 \\ a2 \end{bmatrix}
=
$$

### inline LaTeX
or you can display equations inline $\displaystyle\lim_{x\rightarrow8}\frac{1}{x{-}8}=\infty$
