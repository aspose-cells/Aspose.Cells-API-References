---
title: formula 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 460
url: /zh/python-net/aspose.cells/cell/formula/
is_root: false
---
## formula 属性

获取或设置 [Cell](/cells/zh/python-net/aspose.cells/cell) 的 formula。

### 评论

 formula 字符串始终以等号 (=) 开头。
并且请始终使用逗号（，）作为参数分隔符，例如“=SUM（A1，E1，H2）”。

### 例子

```python
from aspose.cells import Workbook

excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"

```
### 定义：
```python
@property
def formula(self):
    ...
@formula.setter
def formula(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
