---
title: test
date: 2020-12-11T15:00:24.926Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
1. 创建数组
`np.array(list/tuple)`
`np.asarray(list/tuple)`
    - 都是在内存中复制一个新的 `np.ndarray` object
>当数据源本身是一个`ndarray`对象时， np.array(onj) 会复制一个新副本，占用新的内存，
而`np.asarray(obj)`只会返回一个新的pointer指向原来的obj


`np.array(list/tuple, dtype = int64)`
  - 创建特殊的数组
        1. `np.arange(start=0, end(exclusive),step_size=1,dtype)`: `[0,1,...,n-1]`
        2. `np.ones(shape,dtype)`: 全一数组
        3.  `np.zeros(shape,dtype)`
        4. `np.eye(shape,dtype)`: 单位矩阵
        5. `np.linspace(start,stop(inclusive),num元素个数,dtype)`: 等差数列
        6. `np.logspace(起始指数，结束指数，元素个数，base，dtype)`:  等比数列 

2. 数组的属性
    - ndim: dimension of array
    - shape: 数组的形状
    - size: 数组元素的总个数
    - dtype: 数组元素的数据类型
        - NumPy要求数组中所有元素的**数据类型**必须一致
    - itemsize: 数组每个元素的字节数