---
title: placement 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 980
url: /zh/python-net/aspose.cells.drawing/oleobject/placement/
is_root: false
---
## placement 属性

表示绘图对象附加到其下方单元格的方式。
该属性控制工作表上对象的 placement。

### 例子

```python
from aspose.cells.drawing import PlacementType

if shape.placement == PlacementType.MOVE:
    shape.placement = PlacementType.MOVE_AND_SIZE

```
### 定义：
```python
@property
def placement(self):
    ...
@placement.setter
def placement(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [OleObject](/cells/zh/python-net/aspose.cells.drawing/oleobject)
* 类 [PlacementType](/cells/zh/python-net/aspose.cells.drawing/placementtype)
