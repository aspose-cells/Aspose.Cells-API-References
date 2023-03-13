---
title: default_style 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 540
url: /zh/python-net/aspose.cells/workbook/default_style/
is_root: false
---
## default_style 属性

获取或设置工作簿的默认 [Style](/cells/zh/python-net/aspose.cells/style) 对象。

### 评论

DefaultStyle 属性对于为整个工作簿实现样式很有用。

### 例子

以下代码创建并实例化一个新工作簿，并为其设置默认值 [Style](/cells/zh/python-net/aspose.cells/style)。

```python
from aspose.cells import Workbook

workbook = Workbook()
defaultStyle = workbook.default_style
defaultStyle.font.name = "Tahoma"
workbook.default_style = defaultStyle

```
### 定义：
```python
@property
def default_style(self):
    ...
@default_style.setter
def default_style(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Style](/cells/zh/python-net/aspose.cells/style)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
