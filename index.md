---
layout: default
---

## 필요한 패키지
```markdown
from math import factorial
from decimal import Decimal
```

## 테일러급수를 이용해 지수함수를 전개.
```markdown
def exp(p):
    temp=0
    out=0
    while temp<=100:
        out=out+(p**temp)/factorial(temp)
        print(str(format(Decimal.from_float(out), '.1000')))
        temp=temp+1
    print(str(format(Decimal.from_float(out), '.1000')))
```


