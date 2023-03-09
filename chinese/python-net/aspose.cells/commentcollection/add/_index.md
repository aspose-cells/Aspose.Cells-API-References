---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/commentcollection/add/
is_root: false
---
##  add(cell_name) {#str}
向集合添加评论。


### 返回

[Comment](/cells/zh/python-net/aspose.cells/comment) 对象索引。


```python
def add(self, cell_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| cell_name | str | Cell 名称。|

### 例子

```python

commentIndex2 = comments.add("B2")
comment2 = comments[commentIndex2]
comment2.note = "Second note."
comment2.font.name = "Times New Roman"

```


##  add(row, column) {#int-int}
向集合添加评论。


### 返回

[Comment](/cells/zh/python-net/aspose.cells/comment) 对象索引。


```python
def add(self, row, column):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row | int | Cell 行索引。|
| column | int | Cell 列索引。|

### 例子

```python

commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Comment](/cells/zh/python-net/aspose.cells/comment)
* 类 [CommentCollection](/cells/zh/python-net/aspose.cells/commentcollection)
