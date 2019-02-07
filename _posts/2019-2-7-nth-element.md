---
layout: post
title: 'OI学习之stl nth_element()'
subtitle: 'nth_element'
date: 2019-02-07
categories: oi
cover: '../../../assets/img/cpp.jpg'
tags: oi cpp
---
## 位置
```cpp
#include<algorithm>
```
## 签名
1.(default)
```cpp
template <class RandomAccessIterator>
  void nth_element (RandomAccessIterator first, RandomAccessIterator nth,
                    RandomAccessIterator last);
```
2.(custom)
```cpp
template <class RandomAccessIterator, class Compare>
  void nth_element (RandomAccessIterator first, RandomAccessIterator nth,
                    RandomAccessIterator last, Compare comp);
```
## 这是做甚的 ?
使第n大元素处于第n位置（从0开始,其位置是下标为 n的元素），并且比这个元素小的元素都排在这个元素之前，比这个元素大的元素都排在这个元素之后，但不能保证他们是有序的 .
## 方法
```cpp
int a[2000];//int 也可为其他
int nth=20;
// Various operations on array a ...
nth_element(a,a+2000,nth);
```