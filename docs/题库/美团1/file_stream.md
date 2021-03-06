# 文件流

## 题目描述

小团最近在学习操作系统。

文件流是操作系统中一个重要的概念。在 Linux 操作系统中，/dev/random 和 /dev/urandom 是两个重要的设备，它们可以提供永不为空的随机字节数据流。在这里，流是不能回退的。

小团自己也实现了一个类似于 /dev/random 的设备 /dev/crandom，但是它只能提供预先设定好但循环不断的某个由随机小写字母组成的字符串。比如这个随机字符串为 meituan，那么这个设备会提供永不为空的字符串流 meituanmeituanmeit…。

小团想利用这个设备生成一段由小写英文字母组成的文字，但她想知道恰好生成完这段文字时，浪费了这个流的多少个字符。



## 输入描述

第一行一个长为 n 的字符串 s，表示这个循环出现的随机字符串。

第二行一个长为 m 的字符串 a，表示小团想要生成的字符串。

对于 30% 的数据，1≤n, m≤10<sup>3</sup>。

对于另外 20% 的数据，保证 s 串中 ASCII 码大的字母均出现在 ASCII 码小的字母之后。

对于全部数据，1≤n, m≤10<sup>5</sup>，保证字符串 s 与 a 只包含小写英文字母



## 输出描述

输出一行一个整数，如果不能生成字符串 a，则输出 -1，否则输出恰好生成完这个字符串时，浪费了这个流的多少个字符。



## 示例1

输入

> meituan</br>
  uta

输出

> 10

## 提示

拿出生成流中字母的情况如下，拿取的字母用下划线表示。

**<font size = 4>meit<u>u</u>anmei<u>t</u>u<u>a</u>n...</font>**

在生成好最后一个a的时候，浪费了其之前没有标下划线的10个字符。