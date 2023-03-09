---
title: remove_at方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 90
url: /zh/python-net/aspose.cells/commentcollection/remove_at/
is_root: false
---
##  remove_at(cell_name) {#str}
删除特定单元格的注释。



```python
def remove_at(self, cell_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| cell_name | str |包含注释的单元格的名称。|

### 例子

```python

comments.remove_at("B2")

```


##  remove_at(row, column) {#int-int}
删除特定单元格的注释。



```python
def remove_at(self, row, column):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row | int |行索引。|
| column | int |列索引。|

### 例子

```python

comments.remove_at(1, 1)

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [CommentCollection](/cells/zh/python-net/aspose.cells/commentcollection)
