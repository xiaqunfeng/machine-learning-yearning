# Machine Learning Yearning

**目  录**

* [简介](#简介)
* [目的](#目的)
* [翻译章节](#翻译章节)
    * [Setting up development and test sets](#setting-up-development-and-test-sets)
    * [Basic Error Analysis](#basic-error-analysis)
    * [Bias and Variance](#bias-and-variance)
    * [Learning curves](#learning-curves)
    * [Comparing to human-level performance](#comparing-to-human-level-performance)
    * [Training and testing on different distributions](#training-and-testing-on-different-distributions)
    * [Debugging inference algorithms](#debugging-inference-algorithms)
    * [End-to-end deep learning](#end-to-end-deep-learning)
* [英文原文](#英文原文)

## 简介

NG的手稿，还没有出全。我这里边学习边翻译，随手记录之，加深学习印象，仅供学习交流。 

官网：[http://www.mlyearning.org/](http://www.mlyearning.org/)

更好阅读体验，移步gitbook：https://xiaqunfeng.gitbooks.io/machine-learning-yearning/content/

> **声明**：本rep是自己学习过程的一个记录，仅用于学习目的，从未主动宣传和寻求关注过，从默默无闻到被这么多人关注深感荣幸。因为仅仅是随笔形式并从未考虑过商业用途，所以版权意识较弱，没有及时申请授权。我也是今天才知道已经有作者近期取得了商业授权并开源（最近一个月内开源的）。该作者已与我取得联系，首先就被动被报道向取得授权的作者深表歉意，其次我们达成以下共识：1、我将增加LISENSE，修改著作权（没弄过，需要研究一下怎么操作）；2、我已经向Andrew Ng申请仅用于学习交流的授权，待回复；3、后续我也会向取得授权作者仓库贡献自己的一些力量，一起让翻译质量更好。

**更新记录：**

- update 2018.04.25：NG终于出15~19章的手稿啦，等的好辛苦（DONE）

> Tips：在原先的12章和13章之间新增一个章节 `13 Build your first system quickly, then iterate`，原先的chapter13变为14，chapter14变为15

- update 2018.05.02：手稿 20~22 章已出（DONE）
- update 2018.05.09：手稿 23~27 章已出（DONE）
- update 2018.05.16：手稿 28~30 章已出（DONE）
- update 2018.05.23：手稿 31~32 章已出（DONE）
- update 2018.05.30：手稿 33~35 章已出（DONE）
- update 2018.06.06：手稿 36~39 章已出（DONE）
- update 2018.06.13：手稿 40~43 章已出（DONE）
- update 2018.06.20：手稿 44~46 章已出（DONE）
- update 2018.06.27：手稿 47~49 章已出（DONE）
- update 2018.07.04：手稿 50~52 章已出（DONE）

> 业余时间翻译，水平有限，如有不妥或错误之处，欢迎不吝赐教。

## 目的

这本书的目的是教你如何做组织一个机器学习项目所需的大量的决定。 你将学习：

* 如何建立你的开发和测试集

* 基本错误分析

* 如何使用偏差和方差来决定该做什么

* 学习曲线

* 将学习算法与人类水平的表现进行比较

* 调试推理算法

* 什么时候应该和不应该使用端到端的深度学习

* 按步进行错误分析

## 翻译章节

[Chapter 1、Why Machine Learning Strategy](chapter1.md)

[Chapter 2、How to use this book to help your team](chapter2.md)

[Chapter 3、Prerequisites and Notation](chapter3.md)

[Chapter 4、Scale drives machine learning progress](chapter4.md)

### Setting up development and test sets

[Chapter 5、Your development and test sets](chapter5.md)

[Chapter 6、Your dev and test sets should come from the same distribution](chapter6.md)

[Chapter 7、How large do the dev/test sets need to be?](chapter7.md)

[Chapter 8、Establish a single-number evaluation metric for your team to optimize](chapter8.md)

[Chapter 9、Optimizingandsatisficingmetrics](chapter9.md)

[Chapter 10、Having a dev set and metric speeds up iterations](chapter10.md)

[Chapter 11、When to change dev/test sets and metrics](chapter11.md)

[Chapter 12、Takeaways: Setting up development and test sets](chapter12.md)

### Basic Error Analysis

[Chapter 13、Build your first system quickly, then iterate](chapter13.md)

[Chapter 14、Error analysis: Look at dev set examples to evaluate ideas](chapter14.md)

[Chapter 15、Evaluate multiple ideas in parallel during error analysis](chapter15.md)

[Chapter 16、Cleaning up mislabeled dev and test set examples](chapter16.md)

[Chapter 17、 If you have a large dev set, split it into two subsets, only one of which you look at](chapter17.md)

[Chapter 18、How big should the Eyeball and Blackbox dev sets be?](chapter18.md)

[Chapter 19、Takeaways: Basic error analysis](chapter19.md)

### Bias and Variance

[Chapter 20、Bias and Variance: The two big sources of error](chapter20.md)

[Chapter 21、Examples of Bias and Variance](chapter21.md)

[Chapter 22、Comparing to the optimal error rate](chapter22.md)

[Chapter 23、Addressing Bias and Variance](chapter23.md)

[Chapter 24、Bias vs. Variance tradeoff](chapter24.md)

[Chapter 25、Techniques for reducing avoidable bias](chapter25.md)

[Chapter 26、Error analysis on the training set](chapter26.md)

[Chapter 27、Techniques for reducing variance](chapter27.md)

### Learning curves

[Chapter 28、Diagnosing bias and variance: Learning curves](chapter28.md)

[Chapter 29、Plotting training error](chapter29.md)

[Chapter 30、Interpreting learning curves: High bias](chapter30.md)

[Chapter 31、Interpreting learning curves: Other cases](chapter31.md)

[Chapter 32、Plotting learning curves](chapter32.md)

### Comparing to human-level performance

[Chapter 33、Why we compare to human-level performance](chapter33.md)

[Chapter 34、How to define human-level performance](chapter34.md)

[Chapter 35、Surpassing human-level performance](chapter35.md)

### Training and testing on different distributions

[Chapter 36、When you should train and test on different distributions](chapter36.md)

[Chapter 37、How to decide whether to use all your data](chapter37.md)

[Chapter 38、How to decide whether to include inconsistent data](chapter38.md)

[Chapter 39、Weighting data](chapter39.md)

[Chapter 40、Generalizing from the training set to the dev set](chapter40.md)

[Chapter 41、Identifying Bias, Variance, and Data Mismatch Errors](chapter41.md)

[Chapter 42、Addressing data mismatch](chapter42.md)

[Chapter 43、Artificial data synthesis](chapter43.md)

### Debugging inference algorithms

[Chapter 44、The Optimization Verification test](chapter44.md)

[Chapter 45、General form of Optimization Verification test](chapter45.md)

[Chapter 46、Reinforcement learning example](chapter46.md)

### End-to-end deep learning

[Chapter 47、The rise of end-to-end learning](chapter47.md)

[Chapter 48、More end-to-end learning examples](chapter48.md)

[Chapter 49、Pros and cons of end-to-end learning](chapter49.md)

[Chapter 50、Choosing pipeline components: Data availability](chapter50.md)

[Chapter 51、Choosing pipeline components: Task simplicity](chapter51.md)

[Chapter 52、Directly learning rich outputs](chapter52.md)

...

## 英文原文

当前更新到了52章，详见 draft 目录：

01-14章：[Ng_MLY01-01-14.pdf](draft/Ng_MLY01-01-14.pdf)

15-19章：[Ng_MLY02-15-19.pdf](draft/Ng_MLY02-15-19.pdf)

20-22章：[Ng_MLY03-20-22.pdf](draft/Ng_MLY03-20-22.pdf)

23-27章：[Ng_MLY04-23-27.pdf](draft/Ng_MLY04-23-27.pdf)

28-30章：[Ng_MLY05-28-30.pdf](draft/Ng_MLY05-28-30.pdf)

31-32章：[Ng_MLY06-31-32.pdf](draft/Ng_MLY06-31-32.pdf)

33-35章：[Ng_MLY07-33-35.pdf](draft/Ng_MLY07-33-35.pdf)

36-39章：[Ng_MLY08-36-39.pdf](draft/Ng_MLY08-36-39.pdf)

40-43章：[Ng_MLY09-40-43.pdf](draft/Ng_MLY09-40-43.pdf)

44-46章：[NG_MLY10-44-46.pdf](draft/NG_MLY10-44-46.pdf)

47-49章：[NG_MLY11-47-49.pdf](draft/NG_MLY11-47-49.pdf)

50-52章：[Ng_MLY12-50-52.pdf](draft/Ng_MLY12-50-52.pdf)