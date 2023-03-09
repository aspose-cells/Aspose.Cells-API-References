---
title: find方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 290
url: /zh/python-net/aspose.cells/cells/find/
is_root: false
---
##  find(what, previous_cell) {#any-Cell}
查找包含输入对象的单元格。


### 返回

Cell 对象。


```python
def find(self, what, previous_cell):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| what | any |要搜索的对象。<br/>类型应为 int、double、DateTime、string、bool。|
| previous_cell | [Cell](/cells/zh/python-net/aspose.cells/cell) |具有相同对象的上一个单元格。<br/>如果从头开始搜索，这个参数可以设置为空。|
### 评论

如果未找到单元格，则返回 null（无）。

##  find(what, previous_cell, find_options) {#any-Cell-FindOptions}

查找包含输入对象的单元格。


### 返回

Cell 对象。


```python
def find(self, what, previous_cell, find_options):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| what | any |要搜索的对象。<br/>类型应为 int、double、DateTime、string、bool。|
| previous_cell | [Cell](/cells/zh/python-net/aspose.cells/cell) |具有相同对象的上一个单元格。<br/>如果从头开始搜索，这个参数可以设置为空。|
| find_options | [FindOptions](/cells/zh/python-net/aspose.cells/findoptions) |查找选项|
### 评论

如果未找到单元格，则返回 null（无）。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [Cells](/cells/zh/python-net/aspose.cells/cells)
