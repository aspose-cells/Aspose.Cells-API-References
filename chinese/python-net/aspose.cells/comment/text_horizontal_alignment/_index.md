---
title: text_horizontal_alignment 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 190
url: /zh/python-net/aspose.cells/comment/text_horizontal_alignment/
is_root: false
---
## text_horizontal_alignment 属性

获取和设置评论的文本水平对齐方式。

### 例子

```python
from aspose.cells import TextAlignmentType

if comment1.text_horizontal_alignment == TextAlignmentType.FILL:
    comment1.text_horizontal_alignment = TextAlignmentType.CENTER

```
### 定义：
```python
@property
def text_horizontal_alignment(self):
    ...
@text_horizontal_alignment.setter
def text_horizontal_alignment(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Comment](/cells/zh/python-net/aspose.cells/comment)
* 类 [TextAlignmentType](/cells/zh/python-net/aspose.cells/textalignmenttype)
