今天首先讲了多元分类，它是用逻辑回归解决多个分类问题
我们可以通过看y的离散值设置多个分类器


---tu1---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu1.PNG)




处理分类问题的其实和之前的一样，先将数据分为两类，并把这个分类器函数拟合出来


---tu2---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu2.PNG)




这个分类器实际上在计算给定x和theta时，y的值为1的概率

55.过度拟合

过度拟合的问题就是参数过多，但数据样本过少的问题
它区别于欠拟合，过度拟合的图像因为太死板而无法泛化到其他图形当中去


---tu3---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu3.PNG)





在逻辑回归中也同理

减少过度拟合有两个方法，第一个方法就是减少特征的数量（尽量选取游有用特征）

第二个方法就是正则化，用改变参数的全书，从而改变目标函数


我们的正则化，要有一个惩罚因子
惩罚因子就是在代价函数前面加一些值上去


---tu4---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu4.PNG)






我们可以通过假如乘法一项的方式来减少参数对式子的影响
我们要做的就是修改代价函数，来缩小所有的参数，因为我们不知道缩小哪个参数
 所以我们通过后面加一个正则化的例子

---tu5---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu5.PNG)





线性回归中的正则化


---tu6---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu6.PNG)



矩阵方程的正则化


---tu7---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu7.PNG)




讲了线性回归的正则化，也要讲逻辑回归的正则化


---tu8---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu8.PNG)





我们发现线性回归和逻辑回归样子很像，但又因为有个sigmoid函数，所以本质上的函数却是不一样的


---tu9---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu9.PNG)



而求导之后的样子就像如图所示的样子（上图）
到目前为止，我大致掌握了线性回归，逻辑回归，高级优化算法，正则化，在11年的时候老师讲，我可以当个半吊子工程师啦啦啦

接下来我们学习一个非常强大的非线性分类器，不管是线性回归还是逻辑回归，我们都能够通过构造多项式来解决，但实际上还有更为强大的非线性分类器，可以用之解决多项式回归问题


！！！接下来，我们步入神经网络的学习！！！

问题的由来是真的因为我们要拟合的特征有很多



---tu10---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu10.PNG)





它在非线性假设上是一个很好的方法

前向传播的大致框架如下所示


---tu11---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu11.PNG)





我们需要理解每个符号的含义

当然我们也可以用向量化的方式来表示


---tu12---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu12.PNG)





神经网络前向传播的大概框架


---tu13---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu13.PNG)






我们能可以联系起来记忆 当神经网络蒙住前面的复杂东西后其实就是我们的逻辑回归



---tu14---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu14.PNG)





神经网络中的连接方式被称为神经架构，架构指的是不同的神经元的连接方式

下节课就是介绍，神经网络如何计算输入的，非线性函数





我们可以 轻松的表示单层神经网络其实可以表示and&or

通过设置θ0=-30，θ1=20，θ2=20，我们的输出函数就是
：ℎ𝛩(𝑥) = 𝑔(−30 + 20𝑥1 +20𝑥2)


---tu15---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu15.PNG)




我们又知道sigmoid得函数的样子，我们就把y的值，也就是sigmoid的1，0表示逻辑关系
不难得到当我输入x1，和x2时候就可以得到哦得到与操作




---tu16---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu16.PNG)






同理当我们的参数值设为这个的时候可以得到or函数


---tu17---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu17.PNG)






就像我们之前学计算机科学的时候，当我们来表示其他更为复杂的函数的时候，我们可以将简单的与和非，进行组合就能够得到


---tu18---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu18.PNG)




多类分类也同理，输出的可以用一个向量表示，多个意思



---tu19---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20four/img-day4/tu19.PNG)




















































