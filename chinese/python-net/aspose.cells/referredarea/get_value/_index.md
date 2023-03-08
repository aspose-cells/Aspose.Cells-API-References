---
title: get_value方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/referredarea/get_value/
is_root: false
---
##  get_value(row_offset, col_offset) {#int-int}
从该区域的左上角获取具有给定偏移量的单元格值。


### 返回

“#REF！”如果该区域无效；
"#N/A" 如果给定偏移量超出该区域；
否则返回给定位置的单元格值。


```python
def get_value(self, row_offset, col_offset):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row_offset | int |距此区域起始行的行偏移量|
| col_offset | int |距此区域起始行的列偏移量|


##  get_value(row_offset, col_offset, calculate_formulas) {#int-int-bool}
从该区域的左上角获取具有给定偏移量的单元格值。


### 返回

“#REF！”如果该区域无效；
"#N/A" 如果给定偏移量超出该区域；
否则返回给定位置的单元格值。


```python
def get_value(self, row_offset, col_offset, calculate_formulas):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row_offset | int |距此区域起始行的行偏移量|
| col_offset | int |距此区域起始行的列偏移量|
| calculate_formulas | bool |指定引用为公式是否递归计算|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [ReferredArea](/cells/zh/python-net/aspose.cells/referredarea)
