---
title: add_auto_shape方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/
is_root: false
---
##  add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#AutoShapeType-int-int-int-int-int-int}
将自选图形添加到工作表。


### 返回

形状对象。


```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [AutoShapeType](/cells/zh/python-net/aspose.cells.drawing/autoshapetype) |自动形状类型。|
| upper_left_row | int |左上行索引。|
| top | int |表示 Shape 从其左行的垂直偏移量，以像素为单位。|
| upper_left_column | int |左上列索引。|
| left | int |表示 Shape 从其左列的水平偏移量，以像素为单位。|
| height | int |表示Shape的高度，单位为像素。|
| width | int |表示 Shape 的宽度，以像素为单位。|
### 评论

类型不能是 Chart/Comment/Picture/OleObject/Polygon/DialogBox
### 例子


```python
from aspose.cells.drawing import AutoShapeType

# Adds a AutoShape to the worksheet.
autoShape = shapes.add_auto_shape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
