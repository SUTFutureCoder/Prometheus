# 最大能量

## 题目描述

一年一度的宇宙超级运动会在宇宙英雄体育场隆重举行，X星人为这场运动会准备了很长时间，他大显身手的时刻终于要到了，为了保持良好的竞技状态和充沛的体能，X星人准备了N中不同的能量包，虽然每种能量包都有无限个，但是因为同一种能量包使用太多会带来副作用，因此同样的能量包不能同时使用超过两个，也就是说最多同时可以使用两个相同的能量包，每种能量包都有一个重量值和能量值。由于这些能量包的特殊性，必须要完整地使用一个能量包才能发挥功效，否则将失去对应的能量值，考虑到竞技的公平性，竞赛组委会规定每个人赛前补充的能量包的总重量不能超过W，现在需要你编写一个程序计算X星人能够拥有的最大能量值是多少？



## 输入描述

单组输入：
第一行包含两个空格隔开的正整数N,W，其中N<=10^3,W<=10^3。
第二行到第N+1行，每一行包含两个正整数，分别表示每一种能量包的重量和能量值，两个正整数之间用空格隔开，每一种能量包的重量和能量值都是小于等于100的正整数。



## 输出描述

输出一个非负整数表示X星人能够拥有的最大能量值。



## 示例1

输入

> 3 4<br>
  2 4<br>
  1 2<br>
  3 3

输出

> 6

