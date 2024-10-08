---
layout: article
title: 第一篇博客
---

#### 计算机是怎么存数据的

**1、像开关一样**:想象你有一排开关，每个开关可以是开（1）或关（0）。每个开关就是一个 **位（bit）**。

**2、一个开关（1 位）**:只有两个状态，可以表示 2 种不同的东西，比如 "开" 或 "关"。

**3、多个开关（多个位）**：如果你有更多的开关，就能表示更多的东西。例如：

- **2 个开关**：你可以有 4 种组合（00, 01, 10, 11），所以你能表示 4 种不同的东西。
- **3 个开关**：你可以有 8 种组合（000, 001, 010, 011, 100, 101, 110, 111），所以你能表示 8 种不同的东西。

**4、1 个字节（8 个开关）**：如果你有 8 个开关，你可以表示 256 种不同的东西。这个是因为 2 的 8 次方等于 256。所以，一个字节（8 位）可以表示 256 种不同的状态。

#### 为什么是 2 的幂

- 每增加一个开关

  ：可以表示的组合数就翻倍了。这个翻倍的规律就是 2 的幂。例如：

  - 1 个开关：21=22^1 = 221=2 种组合
  - 2 个开关：22=42^2 = 422=4 种组合
  - 3 个开关：23=82^3 = 823=8 种组合
  - 8 个开关：28=2562^8 = 25628=256 种组合

#### 进制

##### 1、十进制（Decimal）

**十进制**是我们最常用的系统，使用数字 0 到 9。

- **例子**：数字 345 表示 300（3 × 100）+ 40（4 × 10）+ 5（5 × 1）。

##### 2、二进制（Binary）

**二进制**只用 0 和 1。例如：

- 例子

  ：二进制的 101 表示：

  - 第一个 1 是 1 × 2^2 = 4
  - 第二个 0 是 0 × 2^1 = 0
  - 第三个 1 是 1 × 2^0 = 1
  - 加起来就是 4 + 0 + 1 = 5（十进制）

所以，二进制的 101 等于十进制的 5。

##### 3、八进制（Octal）

**八进制**使用数字 0 到 7。例如：

- 例子

  ：八进制的 17 表示：

  - 1 × 8^1 = 8
  - 7 × 8^0 = 7
  - 加起来就是 8 + 7 = 15（十进制）

所以，八进制的 17 等于十进制的 15。

##### 4、十六进制（Hexadecimal）

**十六进制**使用数字 0 到 9 和字母 A 到 F。例如：

- 例子

  ：十六进制的 2F 表示：

  - F 是 15（十进制），所以 2F = 2 × 16^1 + 15 × 16^0
  - 2 × 16 = 32
  - 15 × 1 = 15
  - 加起来就是 32 + 15 = 47（十进制）

所以，十六进制的 2F 等于十进制的 47。

总结

**十进制**：你有 10 个不同的玩具，分别编号从 0 到 9。

**二进制**：你只有 2 种玩具（0 和 1），用这些来编号和计数。

**八进制**：你有 8 种玩具，分别编号从 0 到 7。

**十六进制**：你有 16 种玩具，编号从 0 到 9，再加上 A 到 F。









#### 数据类型

1、`byte` 是 Java 中的一种数据类型，它表示一个<u>占用很小存储空间的整数</u>。

想象一个小盒子，这个盒子只能装下一个 0 到 255 的数字（或 -128 到 127 的数字）。这个小盒子就是 `byte` 类型。它占用的空间很小（只有 **<u>8 位</u>**，或者说 1 个字节），所以非常节省内存。

2、`short` 是 Java 中的另一种数据类型，用于表示<u>稍微大一点的整数</u>。

想象一个比 `byte` 大一点的盒子，这个盒子可以装一个数字，范围从 **-32,768 到 32,767**。这个盒子就是 `short` 类型。它比 `byte` 大一些，占用的空间是 **16 位（2 个字节）**。

