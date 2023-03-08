---
title: get_range方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/name/get_range/
is_root: false
---
##  get_range() {#}
如果此名称引用范围，则获取范围。


### 返回

范围。


```python
def get_range(self):
    ...
```




##  get_range(recalculate) {#bool}
如果此名称引用范围，则获取范围


### 返回

范围。


```python
def get_range(self, recalculate):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| recalculate | bool |如果在本次调用之前已经计算过该名称，是否重新计算。|


##  get_range(sheet_index, row, column) {#int-int-int}
如果此名称引用范围，则获取范围。
如果此名称的引用不是绝对的，则不同单元格的范围可能不同。


### 返回

范围。


```python
def get_range(self, sheet_index, row, column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| sheet_index | int |根据工作表索引。|
| row | int |根据行索引。|
| column | int |相应的列索引|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Name](/cells/zh/python-net/aspose.cells/name)
