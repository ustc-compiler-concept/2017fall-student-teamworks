# 14 Teamwork -- Macro

## 项目地址 
[https://github.com/Robert-Lu/teamwork-14-Macro](https://github.com/Robert-Lu/teamwork-14-Macro)

## 组员信息

|  组员  |                Github ID                 |  身份  |
| :--: | :--------------------------------------: | :--: |
| 鲁吴越  | [Robert-Lu](https://github.com/Robert-Lu) |  队长  |
| 李双利  | [agave233](https://github.com/agave233)  |  成员  |
| 罗永平  |    [ypluo](https://github.com/ypluo)     |  成员  |



## 项目简介

本项目主要研究各种宏的特点与优缺点，包括词法级别与语法级别的宏的调研，以及普通宏与 hygienic macro 的区别。

具体而言，本项目会

1. 首先对词法级别的宏做一个简单的总结，以大家熟知的 C 语言作为实例，由于词法级别的宏具有的特性较少，功能局限性也较多，对这一块不做过多的阐述；
2. 对于语法级别的宏，我们计划对 Lisp 和 Rust 的宏进行分析，这两种语言分别是较传统以及较新式的语言，对于他们之间的区别，Lisp 宏中存在的问题，以及新式语言设计中是如何解决这些问题的，进行调研和总结；
3. 对于 hygienic macro 相关问题的调研，可以穿插前两点中 C 语言和 Lisp 语言中宏存在的卫生性问题来进行解读；

## 任务和分工

将任务分为以下模块：

* 词法级别的宏 

  * a. 总结 C 语言的宏的特性 

  * b. 总结 C 语言的宏的局限性

  * c. 结合宏的卫生性讨论

* 语法级别的宏

  * d. 调研 Lisp 宏的特性

  * e. 调研 Rust 宏的特性

  * f. 比较两者以及总结宏机制在程序语言中的发展

  * g. 结合宏的卫生性讨论

* hygienic macro 相关

  * h. 完成宏的卫生性问题的简介

  * i. 相关学术文献的阅读与调研

  * j. 调研卫生宏的特点以及其与普通宏的区别

* 可选

  * h. 在 `c1i` 项目基础上编写代码，来实现一些宏的高级特性，做一些 demo。

经过组内讨论，以上问题部分是相对独立的，也有部分是相互之间有所关联的。所以，我们进行有重叠的分工计划，如下表所示

|  人员  |     主要任务      |  辅助任务   |
| :--: | :-----------: | :-----: |
| 鲁吴越  | a, c, h, i, j | b, d, e |
| 李双利  | a, b, d, f, i | e, g, h |
| 罗永平  | e, f, g, h, i | a, d, j |

## 讨论记录

#### 12月11日 晚

地点：线上讨论组
时间：约 30 分钟
* 成员的自我介绍，关于对项目的初步理解与成员已掌握相关技术的讨论
* 初步讨论了分工与计划

#### 12月13日 午

地点：西区图书馆
时间：约 1 小时
* 对于项目简介的提交进行讨论
* 进一步讨论了各阶段的计划
* 对于词法分析部分的任务进行了讨论与总结，该部分调研任务大致已结束

#### 12月21日 晚

地点：线上讨论组
时间：约 1 小时 30 分
* 对于语法分析部分的任务进行了讨论，该部分仍然需要进一步调研
* 对于任务 i 进行了讨论，交换了对于论文的一些理解

#### 1月1日 晚

地点：线上讨论组
时间：约 1 小时
* 对于相关论文的讨论部分进行了讨论

#### 1月3日 晚

地点：线上讨论组
时间：约 30 分
* 对于项目第二次提交的相关问题进行讨论

## 进展记录

#### 12月13日

* 添加项目简介，完成公共仓库初次提交
* 同时大致完成了词法分析部分的任务

#### 12月20日

* 添加了关于语法分析部分的部分调研进展

#### 12月22日

* 添加了关于宏卫生性问题的部分调研进展

#### 1月2日

* 添加了相关论文的讨论部分

## 遇到的问题

* 研究语言的宏时，是否应该忽略对应语言的本身特性而关注于宏策略
* 如何对于任务 h 的实现难度进行合理评估

## 下一步的计划

* 对任务 h 的实现难度进行合理评估
* 论文的相关讨论还需要一些工作
* 需要调研一到两种除 Lisp 之外的有语法级别宏的语言的宏机制

## 文献及引用

[Herman, David, and Mitchell Wand. "*A theory of hygienic macros.*" ESOP. Vol. 8. 2008.](http://www.ccs.neu.edu/home/dherman/research/papers/esop08-hygiene.pdf)

[Clinger, William. "*Hygienic macros through explicit renaming*." ACM SIGPLAN Lisp Pointers 4.4 (1991): 25-28.](https://dl.acm.org/citation.cfm?id=1317269)

[Rust Documentation 1.7.0 - Macros](https://doc.rust-lang.org/1.7.0/book/macros.html)

[The Common Lisp Cookbook - Macros and Backquote](http://cl-cookbook.sourceforge.net/macros.html)