reference : https://www.bilibili.com/video/BV1KZ4y1v7nA


![1](https://user-images.githubusercontent.com/126434615/227891808-f988718e-bfdf-46e3-b3b3-fb9921d96230.png)


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
\frac{\tan\alpha-\tan\beta} {\Delta x} = \frac {u} {T} \frac{\partial^2 y} {\partial t^2} 
```

