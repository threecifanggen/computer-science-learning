# 第一章 简介

## 1.1 为什么QC重要？

## 1.2 属于定义

### 计算机的定义

> A *computer* is a device that takes data as input and does some sort of operations on that data.

> **计算机**是一个接收输入的数据并基于这些数据进行一些运算的装置。

### 量子计算机的定义

> A *quantum computer* is a device that takes data as input and does some sort of operations on that data with a process that can only be described using quantum physics.

> **量子计算机**是指接收输入的数据，并且执行一些只能用量子物理描述的运算的设备。

传统的量子设备的特点：1. 冷；2.孤立。愿意是为了可以保证不受噪音的影响。

## 1.3 我们将如何使用QC

QC比较适合一些特定领域（作者用了GPU的例子）。

当QC没有特别大的优势的时候，传统计算机还是优先的选择，因为QC具有一些限制。

![](assets/img/2021-12-26-16-56-09.png)

Q Computer需要一些硬件上的限制，需要与环境独立，因此，一个常用的解决方案是接近0K度，这使得这种设备很难在我们的个人设备上使用。

### 1.3.1 Q Computer可以做什么？

* 下面举例一些常用算法：
  1. `Grover`算法：用$\sqrt{N}$布搜索一个具有$N$长度的列表
  2. `Shor`算法：计算大整数的因子（常用在密码学中）
* Q computer可以很好地模拟一些量子系统的特性，这对于化材领域有突破性影响。
* 在一些参数评估、安全方面也有很大作用

### 1.3.2 Q Computer不能做什么？

* 大数据问题不适合量子设备
* 需要大量随机过程数据的机器学习应用也不适合。「平行宇宙」的概念来表述（大量的交互数据是很难的）。

## 1.4 什么是程序？

> A *program* is a sequence of instructions that can be interpreted by a classical computer to perform a desired task. Tax forms, driving directions, recipes, and Python scripts are all examples of programs.

### 1.4.1 什么是量子程序？

![](assets/img/2021-12-26-17-10-55.png)


