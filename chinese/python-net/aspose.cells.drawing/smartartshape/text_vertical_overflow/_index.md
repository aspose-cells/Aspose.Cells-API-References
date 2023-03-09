---
title: text_vertical_overflow 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 1020
url: /zh/python-net/aspose.cells.drawing/smartartshape/text_vertical_overflow/
is_root: false
---
## text_vertical_overflow 属性

获取和设置包含文本的形状的文本垂直溢出类型。

### 例子

```python
from aspose.cells.drawing import TextOverflowType

if shape.text_vertical_overflow == TextOverflowType.CLIP:
    shape.text_vertical_overflow = TextOverflowType.OVERFLOW

```
### 定义：
```python
@property
def text_vertical_overflow(self):
    ...
@text_vertical_overflow.setter
def text_vertical_overflow(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [SmartArtShape](/cells/zh/python-net/aspose.cells.drawing/smartartshape)
* 类 [TextOverflowType](/cells/zh/python-net/aspose.cells.drawing/textoverflowtype)
