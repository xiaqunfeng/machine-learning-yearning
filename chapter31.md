## Chapter 31、Interpreting learning curves: Other cases

**解释学习曲线：其他情况**

考虑如下学习曲线：

![0](http://oow6unnib.bkt.clouddn.com/myl-c31-0.jpg)

该曲线表明高偏差、高方差，还是二者？

蓝色的训练错误曲线相对低，红色开发错误曲线远高于蓝色训练错误。因此，偏差较小，但是方差较大。添加更多训练数据可能有助于缩小开发错误和训练错误之间的差距。

现在，考虑如下：

![1](http://oow6unnib.bkt.clouddn.com/myl-c31-1.jpg)

这次，训练错误较大，远高于期望性能水平。开发错误也比训练错误大很多。因此，具有显著的偏差和方差。你将不得不在算法中去寻找同时减少偏差和方差的方法。