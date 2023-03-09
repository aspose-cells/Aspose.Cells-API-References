---
title: ShapeTextAlignment类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 80
url: /zh/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
## ShapeTextAlignment类
表示形状的文本对齐方式的设置；



ShapeTextAlignment 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [is_text_wrapped](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) |获取和设置包含文本的形状的文本环绕类型。|
| [rotate_text_with_shape](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) |指示是否旋转带有形状的文本。|
| [text_vertical_overflow](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) |获取和设置文本框的文本垂直溢出类型。|
| [text_horizontal_overflow](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) |获取和设置文本框的文本水平溢出类型。|
| [rotation_angle](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) |获取和设置形状的旋转。|
| [text_vertical_type](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) |获取和设置文本方向。|
| [auto_size](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) |指示形状的大小是否根据其内容自动调整。|
| [text_shape_type](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) |获取和设置文本的转换类型。|
| [top_margin_pt](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) |以 Points 为单位返回上边距|
| [bottom_margin_pt](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) |以点为单位返回底部边距|
| [left_margin_pt](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) |以点为单位返回左边距|
| [right_margin_pt](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) |以点为单位返回右边距|
| [is_auto_margin](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) |指示文本框的边距是否自动。|
| [number_of_columns](/cells/zh/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) |获取和设置边框中文本的列数。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

### 也可以看看
* 模块 [aspose.cells.drawing.texts](..)
