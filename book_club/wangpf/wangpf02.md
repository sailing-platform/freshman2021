# 《编码》读书笔记1-6章

## 第1章

这一章有一句话比较颠覆了以往自己对于“编码”一词的理解，以往没有详细的细究到底什么是编码，狭义的将编码和密码等同起来，将编码理解成将简单易懂的内容“加密”。而实际上，==编码就是交流的基础，他应该是易于理解的==。

这一章以“电筒密谈”事件引出了对“编码”的讨论，口头语言、英语词汇、摩斯密码等等都是一种编码，是人类交流的基础。对于计算机而言，则有他自己的一套编码。

## 第2章

第二章开始讲起了摩斯密码，得出的结论点有：

> 1. 码字的数目 = 2^编码位数；
>
> 2. 编码进行适合的组合，得出完整的信息表示。

莫尔斯码发送简单，但是接收后解析困难，解决方案：构建信息与编码的图表。

## 第3章

由于最初的盲文编码过于复杂，布莱叶对其进行了改造，由此引出了布莱叶盲文。

> 1. 布莱叶盲文将字符编码成2×3小格中一个或多个凸起的点；
> 2. 布莱叶编码是二元码，每一个点仅含平滑和凸起两种表现形式；
> 3. “先行码/前置码”或“转义码”概念引入：有数字标识或取消数字标识作用的编码，会改变跟随其后的码字的含义；
> 4. “换码代码”概念引入：6号点为大写标识，它表明其后跟随的字母是大写的。

使用6位二进制码表示出2^6=64种编码表示，并且根据上下文有双重身份。

## 第4章

手电筒：

1. 组成：电池+导线+灯泡+开关（开关对应了0或1）；
2. 原理：电池为电路提供电子，在闭合回路中，电子从电池负极流出，经导线流经灯泡后，又经导线流入正级；
3. 灯泡状态：亮/灭。

> 例子生动形象，读者阅读兴趣被很好的激发，这种电子经导线流动也与信号传输/通讯相契合。

## 第5章

第四章描述的手电筒是一个小的系统结构，局限在一定的范围内，远距离如何通讯？依旧采用电源+导线的方式实现。

1. 如果使用的是高压电源和大灯泡，地球可以成为导线，便可以构建远距离手电筒。基于此可以绕过拐弯实现长距离通信。
2. 距离越远，需要的导线越长，成本高并且电阻大，且需要更强电压。因此，“通讯”的距离就有限。

> 第4和5章的内容实际上是第6章的铺垫。

## 第6章

第六章在第四和第五章的基础上进一步描述了电报系统：

1. 思想：在线的一端做一些动作引起线的另一端发生了特定对应动作。==电磁铁==是电报的基础，一端上开关的闭合引起另一端上的电磁铁产生一些动作，即实现通讯；

2. 原理图：如书中第46页上方原理图所示；

   > 发送端：敲击开关产生点、划莫尔斯码;
   >
   > 接收端：发送端电键按下，电磁铁拉动金属杆下降，松开电键，弹回原来位置，接收点、划信息。

3. ==继电器==：在书中第46页上方原理图中间有一个继电站，其中的继电器系统是实现远距离传输信号的关键。通过继电站，微弱的输入电流被增强，输出为强电流继续传输信号。

