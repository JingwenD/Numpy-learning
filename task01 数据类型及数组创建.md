## 如何区分一维、二维、多维？
```{python}
a = np.array(object) 
print(a.ndim)
```

## 以下表达式运行的结果分别是什么?
### (提示: NaN = not a number, inf = infinity)

```{python}
0 * np.nan
# nan
np.nan == np.nan
# False
np.inf > np.nan
# False
np.nan - np.nan
# nan
0.3 == 3 * 0.1 
# False
# 3 * 0.1 = 0.30000000000000004
```

## 给定一系列不连续的日期序列。填充缺失的日期，使其成为连续的日期序列。
```{python}
import numpy as np
dates = np.arange('2020-02-01', '2020-02-10', 2, np.datetime64)
max = np.max(dates)
min = np.min(dates)
newDate = np.arange(min, max+1, 1, np.datetime64)
print(newDate)
#['2020-02-01' '2020-02-02' '2020-02-03' '2020-02-04' '2020-02-05'
 '2020-02-06' '2020-02-07' '2020-02-08' '2020-02-09']
```
