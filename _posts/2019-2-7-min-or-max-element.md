---
layout: post
title: 'OI学习之stl min_element() & max_element()'
subtitle: 'min_element() & max_element()'
date: 2019-02-07
categories: oi
cover: '../../../assets/img/cpp.jpg'
tags: oi cpp
---
## Where
```cpp
#include<algorithm>
// 还是万能的 algorithm 库
```
## What
1.default
```cpp
template <class ForwardIterator>
  ForwardIterator min_element (ForwardIterator first, ForwardIterator last);
```
```cpp
template <class ForwardIterator>
  ForwardIterator max_element (ForwardIterator first, ForwardIterator last);
```
2.custom
```cpp
template <class ForwardIterator, class Compare>
  ForwardIterator min_element (ForwardIterator first, ForwardIterator last,
                               Compare comp);
```
```cpp
template <class ForwardIterator, class Compare>
  ForwardIterator max_element (ForwardIterator first, ForwardIterator last,
                               Compare comp);
```
返回 max/min 元素在数组中的指针 .
## How
```cpp
int a[10]={0,9,2,6,4,3,5,7,8,1};
int id=binary_search(a,a+10,5);
int* id1=max_element(a,a+10);
int* id2=min_element(a,a+10);
int pos1= id1-a;//指针转下标
int pos2= id2-a;
//这句输出下标
cout<<pos1<<" "<<pos2<<endl;
//这句输出值
cout<<*id1<<" "<<*id2<<endl;
```
Output:  
```
1 0
9 0
```