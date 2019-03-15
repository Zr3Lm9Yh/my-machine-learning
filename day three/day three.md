今天把octave的幼稚操作跑了一遍，不过我却没跟着笔记去实现那个线性回归怎样来的


今天学习的内容是我之前补的坑，也就是再次暴风哭泣我的学习顺序，今天的的学习说实话效率也不是很高诶，不知道为什么，总觉得自己注意力不够集中，感觉应该很快完成的，已经过去了三天，才学习了整个机器学习的1/3，而且octave也用的不是很熟悉，不过我不能跟着自己的想法走，而是要学会自己明白自己掌握了吗，学会了吗


我们之前学习的是线性回归模型，这个模型的话，首先会有一些数据，这些数据就是他的一些影响参数，比如房价
y=Θ。X1+θX2.+一直加完，可以将它整理为一个数组的形式用来表示它，当让我们的目的是找到一条标准的直线用来拟合它，具体的方式，假设我们只有一个参数的话，比如我们只有一个参数影响，首先我们先将目标函数表示清楚后，然后将值带进去后，参生了一个对应的目标值，和原函数值相减的平方，然后求他的最小值，怎样求这个的最小值呢，首先我们代价函数的方程式我们是知道的然后，根据我们的梯度下降法，最开始自定义一个数，然后一步步通过梯度算法，其实就是求偏导一步步算下去


以上的内容呢就是昨天的。
今天我们厉害了，我们开始学习的不是线性回归模型去预测，而是学习的是分类算法
首先对于我们普通线性回归模型显然对于模型不能够很好的概括出


---tu1---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20three/img-day3/tu1.PNG)




所以我们要研究的算法是逻辑回归算法，这个算法的实质是：它的的输出值永远是0和1之间
因为我们要使目标函数的值在0~1


----tu2----
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20three/img-day3/tu2.PNG)




以上内容就是如何判定边界

接下来我们接着看代价函数
因为在线性回归模型我们定义的代价函数是一个凸函数，而这个我们经过sigmoaid所以就不能用以前的，这就意味着我们需要对图像
进行一些处理，使图像变得不是非凸图像


----tu3---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20three/img-day3/tu3.PNG)




最后我们将图像化简后，变得到了我们图像最后的样子


---tu4---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20three/img-day3/tu4.PNG)




当然我们可以用简单一点的方法来表示代价函数
就是将


---tu5---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20three/img-day3/tu5.PNG)




最后我们通过先前更新参数的方式，更新参数，但是你要知道他们两个根本不是一回事


----tu6----
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20three/img-day3/tu6.PNG)




---tu7---
![ad](https://github.com/Zr3Lm9Yh/my-machine-learning/blob/master/day%20three/img-day3/tu7.PNG)






