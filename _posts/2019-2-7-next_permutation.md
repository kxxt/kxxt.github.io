---
layout: post
title: 'OI学习之stl next_permutation()'
subtitle: 'next_permutation'
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
```cpp
#include <algorithm>
bool next_permutation( iterator start, iterator end );
//The next_permutation() function attempts to transform the given range of elements [start,end) into the next lexicographically greater permutation of elements. If it succeeds, it returns true, otherwise, it returns false.
```
## 方法
1. c++
```cpp
#include <iostream>
#include <algorithm>
#include <string>

using namespace std;

int main()
{
    string str;
    cin >> str;
    sort(str.begin(), str.end());
    cout << str << endl;
    while (next_permutation(str.begin(), str.end()))
    {
        cout << str << endl;
    }
    return 0;
}
```
2. c
```c
#include <cstdio>
#include <algorithm>
#include <cstring>
#define MAX 100

using namespace std;

int main()
{
    int length;
    char str[MAX];
    gets(str);
    length = strlen(str);
    sort(str, str + length);
    puts(str);
    while (next_permutation(str, str + length))
    {
        puts(str);
    }
    return 0;
}
```