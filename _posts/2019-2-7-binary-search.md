---
layout: post
title: 'OI学习之stl binary_search()'
subtitle: 'binary_search'
date: 2019-02-07
categories: oi
cover: '../../../assets/img/cpp.jpg'
tags: oi cpp
---
# STL 的 binary_search()
> 本文介绍的是std::binary_search() , 而不是手写的二分查找代码 .
## Where
```cpp
#include<algorithm>
```
## What
1.(default)
```cpp
template <class ForwardIterator, class T>
  bool binary_search (ForwardIterator first, ForwardIterator last,
                      const T& val);
```
2.(custom)
```cpp
template <class ForwardIterator, class T, class Compare>
  bool binary_search (ForwardIterator first, ForwardIterator last,
                      const T& val, Compare comp);
```
## How
该方法返回找到还是未找到  .
```cpp
int a={0,1,3,4,5,9,8,7,6,2};
int something_to_search=6;
bool found=binary_search(a,a+10,something_to_search);
```