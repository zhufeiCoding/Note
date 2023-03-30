reference : https://www.bilibili.com/video/BV1KZ4y1v7nA


![1](https://user-images.githubusercontent.com/126434615/228120601-5a475d70-ed1a-4a4a-a503-7d873956da11.png)


T1 T2 拉力


$\alpha$  和 $\beta$ 为夹角

### 由牛顿第二定律得:

    1,水平方向上的合力为 0
```math
\sum_{x}^{}F_x=0
```

```math
T_1\cos\alpha-T_2\cos\beta=0
```
    2,垂直方向上的合力为ma

```math
\sum_{u}^{}F_u=ma
```


```math
T_1\sin\alpha-T_2\sin\beta=ma

```
 
#### 我们令
```math
T_1\cos\alpha=T_2\cos\beta=T  (公式1)
```

因为加速度是速度对时间的微分， 而速度是长度对时间的微分， 所以我们可以写成以下形式。
```math
T_1\sin\alpha-T_2\sin\beta=ma=m\frac{\partial^2 y}{\partial t^2}  (公式2)
```



#### 我们设 u 为线密度。则 u可以表示为 线的总质量 除以 线的总长度

```math
u = \frac {M} {L}
```

令线上每一微小的一段质量为 $\Delta M$ , 每一微小一段质量为 $\Delta L$, 则：

```math
\frac {\Delta M} {\Delta L} = \frac {m} {PQ}   
```
这里的PQ就是上图中每一微小的弧长， 我们可以令弧长约等于 $\Delta x$ , 可得：

```math
\frac {\Delta M} {\Delta L} = \frac {m} {PQ}   \approx \frac {m} {\Delta x}
```

我们于是得到：
```math
m \approx u \Delta x

```

### 现在我们可以把公式1，公式2重新整理成公式3，公式4


```math
T_1\cos\alpha=T_2\cos\beta=T  (公式3)
```

```math
T_1\sin\alpha-T_2\sin\beta=ma=u \Delta x\frac{\partial^2 y}{\partial t^2}  (公式4)
```

接下来我们对公式4的两边同时除以T，即公式1的对应项。得：

```math
\frac{T_1\sin\alpha}{T_1\cos\alpha} - \frac{T_2\sin\beta}{T_2\cos\beta} = \frac{u}{T}\Delta x\frac{\partial^2 y}{\partial t^2}
```

我们把对应相同的系数约掉，得：

```math
\frac{\tan\alpha-\tan\beta} {\Delta x} = \frac {u} {T} \frac{\partial^2 y} {\partial t^2}   (公式5)
```




### $\tan\alpha$ $\tan\beta$ 的定义

```math
\tan\alpha = y'_x(x,t)|_{x=x+\Delta t}   = \frac{\partial y} {\partial x} |_{x=x+\Delta x}   (公式6)
```

```math
\tan\beta = y'_x(x,t)|_{x=x}  = \frac{\partial y} {\partial x} |_{x=x}           (公式7)
```



#### 把公式6，7代入公式5得：

```math
\frac{y'_x(x,t)|_{x=x+\Delta t}  -  y'_x(x,t)|_{x=x} }{\Delta x} = y''_{xx}(x,t)  (公式8)
```

#### 把公式8的右边带入公式5的左边得：

```math
\frac{\partial^2 y} {\partial x^2}   = \frac {u}{T}  \frac{\partial^2 y} {\partial t^2}  (公式9)

```
至此我们得到了大名鼎鼎的波动方程.





### 我们看一下$\frac{u}{t}$的单位是怎样的。

u 是线密度，所以u的单位为：
```math
\frac {质量}{长度}
```

T 是张力，根据牛顿第二定律f=ma, 其单位为： 
```math
质量*\frac{长度}{时间^2}
```

所以 $\frac{u}{t}$ 的单位为：

```math
\frac {1} { ({\frac {长度} {时间} }) ^ 2}

```

我们令  $\frac{长度}{时间} = C $
则公式9可以整理成：

```math
\frac{\partial^2 y} {\partial x^2}   = \frac {1}{C^2}  \frac{\partial^2 y} {\partial t^2}   (公式10)

```

我们对公式10右边进行整理 并 令其等于 f(x)：

```math
 \frac{\partial y} {\partial t} \approx \frac{y(t,x) - y(t-\Delta t, x)}{\Delta t} = f(t, x)  (公式11)
```

y对于t的两次导数可以表示成

```math
 \frac{\partial^2 y} {\partial t^2} = \frac{\partial f}{\partial t} \approx \frac{f(t+\Delta t,x) - f(t, x)}{\Delta t}    (公式12)

```

我们把公式11带入公式12得：
```math
 \frac{\partial^2 y} {\partial t^2} =\frac{f(t+\Delta t,x) - f(t, x)}{\Delta t}  = \frac{y(t+\Delta t, x) -y(t,x) -y(t,x) +y(t-\Delta t, x)}{\Delta t^2}  = \frac{y(t+\Delta t, x) -2y(t,x) +y(t-\Delta t, x)}{\Delta t^2}   (公式13)
```


同理，我们可得：
```math
\frac{\partial^2 y} {\partial x^2} = \frac{y(t, x+\Delta x) -2y(t,x) +y(t, x-\Delta x)}{\Delta x^2}   (公式14)

```
由公式13 和 公式14 得：

```math

 y(t+\Delta t, x) = \frac{y(t, x+\Delta x) -2y(t,x) +y(t, x-\Delta x)}{\Delta x^2} \frac{T}{u} \Delta t^2 + 2y(t,x) - y(t-\Delta t, x)  (公式15)

```

如下图所示，我们要求黄色点y的值，则需要根据蓝白红三个点求出！

![2](https://user-images.githubusercontent.com/126434615/228233866-970fffa9-ea63-4b04-9644-106507957a42.png)


