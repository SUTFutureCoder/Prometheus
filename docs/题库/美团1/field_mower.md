# 割草机

## 题目描述

小团作为园艺部的一员，主要负责割草的工作。

学校有一块 n×m 大小的草地，这块草地被平均划分为 n×m 个 1×1 的草地块。第 i 行第 j 列的草地块表示为 (i, j)。

接下来 k 天的每天早上，小团都会去割草作为早锻炼项目。起初每个草地块都有一单位的草，每天早上小团都会用割草机将满足 (i - x)<sup>2</sup> + (j - y)<sup>2</sup>≤ r<sup>2</sup> 的所有草地块 (i, j) 中的草全部割掉，也就是让这个草地块中的草数量变为 0。其中 (x, y) 是小团所处的草地块位置，r 对于每天割草是个常数。每过一天，每块草地中草的数量都增加 1。

所有部员打算在第 k 天晚上一起把这片草地上的草全部割完。请问这天晚上会割掉多少单位的草？



## 输入描述

第一行两个整数 n, m，表示草地的大小。

第二行一个整数 k，表示天数。

接下来 k 行，每行三个整数 x, y, r (1 < x < n, 1 < y < m)，分别表示小团所处的草地位置 (x, y) 和参数 r。保证割草的范围不会超出这块草地，也就是 1 ≤ r ≤ min(x – 1, y – 1, n – x, m – y)。

对于 30% 的数据，n, m ≤ 10<sup>3</sup>；

对于 100% 的数据，1 ≤ n, m ≤ 10<sup>5</sup>, 1 ≤ k ≤ 100。

## 输出描述

输出一行一个整数，表示第 k 天晚上割掉的草有多少。



## 示例1

输入

> 6 6</br>
  3</br>
  4 4 2</br>
  3 3 2</br>
  2 4 1</br>

输出

> 68


