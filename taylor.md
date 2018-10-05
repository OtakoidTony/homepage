---
layout: default
---

## 테일러 급수

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

```
html header: <script type="text/javascript"  src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script> 

\\({e}^{i\pi}+1=0\\)
```

$$ x = \frac{-b \pm \sqrt{b^2-4ac}}{2a} $$

$ T_f(x)=\sum_{n=0}^\infty \frac{f^{(n)}(a)}{n!} \, (x-a)^n=f(a) + f'(a)(x-a) + \frac12f''(a)(x-a)^2 + \frac16f'''(a)(x-a)^3 + \cdots $
