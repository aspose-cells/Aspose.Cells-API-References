---
title: calculation_id 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 50
url: /zh/python-net/aspose.cells/formulasettings/calculation_id/
is_root: false
---
## calculation_id 属性

指定用于计算工作簿中的值的计算引擎的版本。

### 评论

此属性仅用于将设置保存到生成的电子表格文件中
以便其他应用程序（例如 ms excel）在加载和操作生成的文件时可以相应地采取行动。
以ms excel为例，如果这个属性的值小于关联的重新计算引擎标识符
使用打开结果文件的应用程序，应用程序将重新计算所有公式的结果
加载文件后立即在此工作簿上。
出于对大多数用户应用程序性能的考虑，我们不会自动计算工作簿上的任何公式，
无论为此属性设置了什么值。
### 定义：
```python
@property
def calculation_id(self):
    ...
@calculation_id.setter
def calculation_id(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [FormulaSettings](/cells/zh/python-net/aspose.cells/formulasettings)
