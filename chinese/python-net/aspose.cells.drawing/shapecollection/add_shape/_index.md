---
title: add_shape方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 260
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_shape/
is_root: false
---
##  add_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#MsoDrawingType-int-int-int-int-int-int}
将形状添加到工作表。


### 返回

形状对象。


```python
def add_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/zh/python-net/aspose.cells.drawing/msodrawingtype) | Mso 绘图类型。|
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
from aspose.cells.drawing import MsoDrawingType

# Add a shape of the specified type
shapeByType = shapes.add_shape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
