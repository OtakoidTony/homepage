---
layout: default
---

## 테일러 급수

$ T_f(x)=\sum_{n=0}^\infty \frac{f^{(n)}(a)}{n!} \, (x-a)^n=f(a) + f'(a)(x-a) + \frac12f' '(a)(x-a)^2 + \cdots $

```python
from math import factorial
from decimal import Decimal

def exp(p):
    temp=0
    out=0
    while temp<=100:
        out=out+(p**temp)/factorial(temp)
        print(str(format(Decimal.from_float(out), '.1000')))
        temp=temp+1
    print(str(format(Decimal.from_float(out), '.1000')))
```


