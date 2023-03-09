---
title: calculate_on_open 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells/formulasettings/calculate_on_open/
is_root: false
---
## calculate_on_open 属性

指示应用程序是否需要在工作簿打开时执行完整计算。

### 评论

此属性仅用于将设置保存到生成的电子表格文件中
以便其他应用程序（例如 ms excel）在加载结果文件时可以相应地执行操作。
出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，
无论为此属性设置了什么值。
### 定义：
```python
@property
def calculate_on_open(self):
    ...
@calculate_on_open.setter
def calculate_on_open(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [FormulaSettings](/cells/zh/python-net/aspose.cells/formulasettings)
