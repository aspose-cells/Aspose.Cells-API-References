---
title: active_x_control 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 240
url: /zh/python-net/aspose.cells.drawing/dialogbox/active_x_control/
is_root: false
---
## active_x_control 属性

获取 ActiveX 控件。

### 例子

```python
from aspose import pycore
from aspose.cells.drawing.activexcontrols import CheckBoxActiveXControl

checkBox1 = pycore.cast(CheckBoxActiveXControl, shape.active_x_control)
# The font name of CheckBox
fontName = checkBox1.font.name

```
### 定义：
```python
@property
def active_x_control(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ActiveXControl](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* 类 [DialogBox](/cells/zh/python-net/aspose.cells.drawing/dialogbox)
