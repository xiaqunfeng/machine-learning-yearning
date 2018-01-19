## Chapter 9、Optimizing and satisficing metrics

**优化指标和满足指标**

这里有组合多个评估指标的另一种方法。

假设你同时关心算法的准确率和运行时间。你需要在如下三个分类器中进行选择： 
![这里写图片描述](http://oow6unnib.bkt.clouddn.com/myl-c9-0.jpg)
如果将准确率和运行时间通过如下一个公式得到单个评估指标会看起来不太自然，例如：

```
Accuracy − 0.5∗RunningTime
```

你可以这样做：首先，定义一个“acceptable”的运行时间。例如任何运行时间在100ms以内的算法都是可接受的。然后，根据满足运行时间标准的分类器，最大化准确率。这里，运行时间就是一个“satisficing metric”，你的分类器必须要在这个指标上表现地“good enough”就行，这就意味着它最多为100ms。准确率是一个“optimizing metric”。

如果你正在权衡N个不同的标准，例如模型的二进制文件大小（这对于移动app很重要，因为用户不想要下载很大的app）、运行时间和准确率，你可以考虑将其中N-1个标准设置为为“satisficing”指标。也就是说你只需要他们满足特定的值即可。然后将最后一个定义为“optimizing”指标。例如，将二进制文件大小和运行时间设定一个可接受的阈值，并尝试在这些约束条件下不断优化准确率。

作为最后一个例子，假定你正在构建一个硬件设备，该设备使用麦克风监听用户说出的某个特定的“唤醒语（wakeword）”，从而唤醒系统。例如：Amazon Echo监听“Alexa”；苹果Siri监听“Hey Siri”；Android监听“Okay Google”；百度app监听“Hello Baidu”。你同时关心假正例的比率（the false positive rate——当没有人说唤醒语时系统唤醒的频率）和假反例的比率（the false negative rate——当有人说出唤醒语时系统没有唤醒的频率）。该系统性能的一个合理目标是最大限度的减少误报率（optimizing metric），同时满足每24小时操作出现不超过一个假正例（satisficing metric）.

一旦你的团队按照评估指标进行优化，他们将能够取得更快的进展。
