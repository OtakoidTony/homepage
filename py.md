---
layout: default
---

## 궤도 시각화

```python
import matplotlib as mpl
from mpl_toolkits.mplot3d import Axes3D
import numpy as np
import matplotlib.pyplot as plt
import math

def normal():
    mpl.rcParams['legend.fontsize'] = 10
    fig = plt.figure()
    ax = fig.gca(projection='3d')
    xv = int(input("x축 속도:"))
    yv = int(input("y축 속도:"))
    zv = int(input("z축 속도:"))
    firstx = int(input("x축 초기값:"))
    firsty = int(input("y축 초기값:"))
    firstz = int(input("z축 초기값:"))
    ac = 10
    zerotime = (2*zv+((4*zv*zv+(8*firstz*ac))**0.5))/(2*ac)
    time = np.linspace(0, zerotime, zerotime)
    z = firstz+(zv*time)-(0.5*ac*time*time)
    x = firstx+(xv*time)
    y = firsty+(yv*time)
    ax.plot(x, y, z, label='물리')
    ax.legend()
    plt.show()




def sgn(x):
    x = int(x)
    if x < 0:
        return -1
    elif x == 0:
        return 0
    else:
        return 1


def wind():
    mpl.rcParams['legend.fontsize'] = 10
    fig = plt.figure()
    ax = fig.gca(projection='3d')

    xv = int(input("x축 속도:"))
    yv = int(input("y축 속도:"))
    zv = int(input("z축 속도:"))
    firstx = int(input("x축 초기값:"))
    firsty = int(input("y축 초기값:"))
    firstz = int(input("z축 초기값:"))
    windtimeinput = float(input("바람부는 시간:"))
    windx = int(input("x축 기준으로 바람이 부는 속도:"))
    windy = int(input("y축 기준으로 바람이 부는 속도:"))
    ac = 10
    zerotime = (2 * zv + ((4 * zv * zv + (8 * firstz * ac)) ** 0.5)) / (2 * ac)

    print("========================")
    print("x축 초기값:", firstx)
    print("y축 초기값:", firsty)
    print("z축 초기값:", firstz)
    print("x축 속도:", xv)
    print("y축 속도:", yv)
    print("z축 속도:", zv)
    print("========================")
    print("바람이 부는 시간", windtimeinput)
    print("공이 지면에 닿는 시간", zerotime)
    print("========================")

    time = np.linspace(0, zerotime, 10000)


    windtime=time

    print(windtime)
    temp = 0
    windtimeinput=windtimeinput*10000/zerotime
    while temp <= windtimeinput:
        windtime[temp] = 0
        temp = temp + 1

    print(windtime)

    x = firstx + (xv * time) + (windx * windtime)
    y = firsty + (yv * time) + (windy * windtime)
    z = firstz + (zv * time) - (0.5 * ac * time * time)

    ax.plot(x, y, z)
    ax.legend()
    plt.show()



wind()

```
[back](./)
