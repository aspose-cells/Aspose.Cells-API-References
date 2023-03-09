---
title: text_vertical_alignment 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 1010
url: /zh/python-net/aspose.cells.drawing/rectangleshape/text_vertical_alignment/
is_root: false
---
## text_vertical_alignment 属性

获取和设置形状的文本垂直对齐类型。

### 例子

```python
from aspose.cells import TextAlignmentType

if shape.text_vertical_alignment == TextAlignmentType.BOTTOM:
    shape.text_vertical_alignment = TextAlignmentType.CENTER

```
### 定义：
```python
@property
def text_vertical_alignment(self):
    ...
@text_vertical_alignment.setter
def text_vertical_alignment(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [RectangleShape](/cells/zh/python-net/aspose.cells.drawing/rectangleshape)
* 类 [TextAlignmentType](/cells/zh/python-net/aspose.cells/textalignmenttype)
