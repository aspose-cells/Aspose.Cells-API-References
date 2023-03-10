---
title: add_active_x_control方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/
is_root: false
---
##  add_active_x_control(type, top_row, top, left_column, left, width, height) {#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int}
创建一个 Activex 控件。


### 返回




```python
def add_active_x_control(self, type, top_row, top, left_column, left, width, height):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | aspose.cells.drawing.activexcontrols.ControlType |控件的类型。|
| top_row | int |左上行索引。|
| top | int |表示 Shape 从其左行的垂直偏移量，以像素为单位。|
| left_column | int |左上列索引。|
| left | int |表示 Shape 从其左列的水平偏移量，以像素为单位。|
| width | int |表示 Shape 的宽度，以像素为单位。|
| height | int |表示Shape的高度，单位为像素。|

### 例子

```python
from aspose.cells.drawing.activexcontrols import ControlType

# add an ActiveX control
activeXControl = shapes.add_active_x_control(ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)
