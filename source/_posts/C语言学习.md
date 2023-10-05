---
title: C语言学习
date: 2023-10-05 19:23:48
tags:
---
# 计算圆的面积

## 题目介绍
本题要求计算圆的面积
此处使用`#define`规定PI为圆周率，并且使用`double`类型存储变量，防止精度丢失


## 代码展示

```C
#include <stdio.h>
#define PI 3.14
double Area(int r)
{
    double S;
    S = PI * r * r;
    return S;
}
int main()
{
    double S;
    int r;
    printf("请输入半径的值\n");
    scanf("%d", &r);
    S = Area(r);
    printf("面积为%lf", S);
    return 0;
}
```