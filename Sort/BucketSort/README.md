# 桶排序

相比于之前的那些基于对比的排序，桶排主要基于分布，采用的是"分配","收集"的想法。

桶排的思想很简单，将数据先分为有顺序的桶，然后，在各自的桶内再排序。

一种可行的操作如下：

```c
12 13 22 23
```

先分为(按照10位数的数字)

```c
12 13
```

```c
22 23
```

之后，在各自的桶里再进行排序。
这样的时间复杂度为O(n)，但是这样的方法却对于数据有很高的要求。

实例中，给的是使用了堆排序的桶排序。