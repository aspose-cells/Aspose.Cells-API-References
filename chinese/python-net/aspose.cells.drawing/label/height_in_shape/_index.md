---
title: height_in_shape 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 440
url: /zh/python-net/aspose.cells.drawing/label/height_in_shape/
is_root: false
---
## height_in_shape 属性

表示形状相对于父形状上边框的垂直偏移量，以父形状高度的 1/4000 为单位。

### 评论

仅当此形状位于组或图表中时适用。

### 例子

```python

if shape.upper_delta_y == 4000:
    shape.upper_delta_y = 2000

```
### 定义：
```python
@property
def height_in_shape(self):
    ...
@height_in_shape.setter
def height_in_shape(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [Label](/cells/zh/python-net/aspose.cells.drawing/label)
