---
title: add_arc方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_arc/
is_root: false
---
##  add_arc(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
将 ArcShape 添加到工作表。


### 返回

一个 ArcShape 对象。


```python
def add_arc(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| upper_left_row | int |左上行索引。|
| top | int |表示 ArcShape 从其左行开始的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示 ArcShape 与其左列的水平偏移量，以像素为单位。|
| height | int |表示 ArcShape 的高度，以像素为单位。|
| width | int |表示 ArcShape 的宽度，以像素为单位。|

### 例子

```python

# add a arc
arcShape = shapes.add_arc(1, 0, 1, 0, 100, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
