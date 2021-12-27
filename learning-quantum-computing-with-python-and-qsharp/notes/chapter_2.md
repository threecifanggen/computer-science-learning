# 第二章: `Qubits`

本书中使用的交互方式：

![](assets/img/2021-12-26-17-13-52.png)

第一个应用：**QRNG**(quantum random number generator)。

## 2.1 为什么我们需要随机数？

哪些领域需要随机：

1. 玩游戏
2. 模拟复杂系统（股票交易）
3. 选择安全的加密方法

如果使用了一个不好的的随机生成器，则很有可能被预测及被攻击。如果使用了正确的方式，QRNG将会被物理规律所保障，而不是计算机多久可以解决这一难题。

QRNG的步骤：

1. 告诉QD声明一个`qubit`。
2. 应用一个*Hadamard instruction*到`qubit`上。
3. 测量`qubit`并返回结果。

## 2.2 什么是传统比特？

使用*bit*这个词的原因是：

1. 任何物理系统都可以用回答是/否的问题描述
2. 信息使用这种物理系统储存

### 2.2.1 我们可以用传统比特做什么？

使用`NOT`运算/门可以做的事：

![](assets/img/2021-12-26-17-27-07.png)

我们可以用两点之间的线上的点描述随机性：

![](assets/img/2021-12-26-17-28-02.png)

### 2.2.2 抽象是我们的朋友

真值表

## 2.3 Qubits：状态和运算/操作

### 2.3.1 qubit的状态

用狄拉克符号($\left<1\right|$和$\left|0\right>$)表述：

![](assets/img/2021-12-26-17-35-16.png)

### 2.3.1 运算/操作的游戏


`NOT`运算可以描述为旋转180°：

$$
\text{NOT} \left| 0 \right> = \left| 1 \right>
$$

![](assets/img/2021-12-26-17-40-29.png)

任意角度都可以下面公式表示

$$
cos(\theta / 2) \left| 0 \right> + sin(\theta / 2) \left| 0 \right>
$$

同事，亦可以用线性组合子表示这个操作：

$$
    cos(\theta / 2) \left| 0 \right> + sin(\theta / 2) \left| 0 \right>  = 
    cos(\theta / 2) \begin{bmatrix} 1 \\ 0 \end{bmatrix} + sin(\theta / 2) \begin{bmatrix} 0 \\ 1 \end{bmatrix} \\
    = \begin{bmatrix} cos(\theta / 2) \\ cos(\theta / 2) \end{bmatrix}
$$

![](assets/img/2021-12-26-17-54-04.png)

### 2.3.3 测量qubits

测量的结果永远是一个经典bit。如过用图表示，就是如下测量乃是看点在Z轴上的投影，看接近哪个。

![](assets/img/2021-12-26-17-56-54.png)

对投射长度的平方描述我们在这个方向测量到状态的可能性。

![](assets/img/2021-12-26-18-00-53.png)

### 2.3.4 泛化测量：基的独立性

$\left< 1|x \right>$表示$\left|x \right>$在$\left< 1 \right|$的投影，即对$\left|x \right>$在$\left< 1\right|$方向的测量。$|\left< 1|x \right>|^2$则表示测量的概率（也叫做Born规则）。

![](assets/img/2021-12-26-18-09-00.png)
![](assets/img/2021-12-26-18-09-10.png)

Qubit具有如下性质：

1. 可以通过向量知识完美地模拟
2. 系统可以用量子运算转换
3. 系统的测量产生一个单独的经典信息比特，遵循Born规则

