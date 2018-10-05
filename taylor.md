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
\[ \vec{\nabla} \times \vec{F} = \left( \frac{\partial F_z}{\partial y} - \frac{\partial F_y}{\partial z} \right) \mathbf{i}
        + \left( \frac{\partial F_x}{\partial z} - \frac{\partial F_z}{\partial x} \right) \mathbf{j} + \left( \frac{\partial
        F_y}{\partial x} - \frac{\partial F_x}{\partial y} \right) \mathbf{k} \]
\[ \vec{\nabla} \times \vec{F} = \left( \frac{\partial F_z}{\partial y} - \frac{\partial F_y}{\partial z} \right) \mathbf{i}
        + \left( \frac{\partial F_x}{\partial z} - \frac{\partial F_z}{\partial x} \right) \mathbf{j} + \left( \frac{\partial
        F_y}{\partial x} - \frac{\partial F_x}{\partial y} \right) \mathbf{k} \]

$$ x = \frac{-b \pm \sqrt{b^2-4ac}}{2a} $$

$x^2$
