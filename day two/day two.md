# my-machine-learning day 2
今天学习了线性回归的适用在多个变量的版本，本质上就是引入向量来存取多个特征，用一个向量来存取参数，这里要注意的是关于一些符号，比如在X（x是用来表示数据的）头上的表示行数的索引，也就是第几行的样本数据，下面的代表第几个数据的索引
最后我们的目标函数就变成两个向量的乘积了
当然了今天温习了下向量的乘积，我们成绩的时候注意是对参数，也就是我们要求的数据进行转置

通过向量参数的封装后，目标函数，代价函数和梯度下降函数就变成了这个歌样子


---tu1---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20two/img-day2/tu1.PNG)

---tu2---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20two/img-day2/tu2.PNG)

---tu3---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20two/img-day2/tu3.PNG)
注意了，这里的求导出来，那你要想怎样来的，沃恩知道一元参数求导，是通过倒数，当然这个多元的话就是偏导数具体的位置的话是我们的笔记中
步骤如图


---tu4---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20two/img-day2/tu4.PNG)

当然了我们再用梯度下降的时候，我们为了使我们收敛速度，合适，所以我们要学会特征缩放


---tu5---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20two/img-day2/tu5.PNG)

将特征的参数取到-1到1之间

当然也可以用均质化归一的思想来初始您的参数
当然优化的时候也要看看阿尔法的参数问题
还有我们也要善于寻找比较好的特征和多项式，你知道的好的特征和多项式可以较好的拟合模型
还有种情况是图形不像标准的线性回归图像，我们就可以将三次函数当作x3的特征参数
来表示


如果你觉得还是很复杂，那么我们换个算法，就是下面要总结的正规方程（区别迭代算的直接解法）


---tu6---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20two/img-day2/tu6.PNG)


首先还是，将X（特征）转化为向量，将y也就是目标的值转化为向量
通过 矩阵的乘法就可以求得最小化代价函数（参数）的矩阵
当然我们的梯度下降和正则化有优缺点比较的（吴恩达老师有个比较图）



---tu7---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20two/img-day2/tu7.PNG)

正规方程以及不可逆的情况，比如说有两个数据有着线性联系（详情参照线性代数）

接下来就是octave挖坑（也就是matlap的用法）为明天挖坑呐

