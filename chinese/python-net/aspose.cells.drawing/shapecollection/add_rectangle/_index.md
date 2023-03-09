---
title: add_rectangle方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 240
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_rectangle/
is_root: false
---
##  add_rectangle(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
将 RectangleShape 添加到工作表。


### 返回

一个 RectangleShape 对象。


```python
def add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| upper_left_row | int |左上行索引。|
| top | int |表示 RectangleShape 从其左行开始的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示 RectangleShape 与其左列的水平偏移量，以像素为单位。|
| height | int |表示 RectangleShape 的高度，以像素为单位。|
| width | int |表示 RectangleShape 的宽度，以像素为单位。|

### 例子

```python

#  add a rectangle
rectangleShape = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
