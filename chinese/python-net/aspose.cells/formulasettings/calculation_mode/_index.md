---
title: calculation_mode 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 60
url: /zh/python-net/aspose.cells/formulasettings/calculation_mode/
is_root: false
---
## calculation_mode 属性

获取或设置 ms excel 中工作簿计算的模式。

### 评论

此属性仅用于将设置保存到生成的电子表格文件中
以便其他应用程序（例如 ms excel）在加载和操作生成的文件时可以相应地采取行动。
出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，
无论为此属性设置了何种模式。
如果用户需要计算公式，请始终根据需要在不同的对象上调用方法：
[Workbook.calculate_formula()](/cells/python-net/aspose.cells/workbook/calculate_formula), [Worksheet.calculate_formula(formula)](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[Cell.calculate(options)](/cells/zh/python-net/aspose.cells/cell/calculate), ...等
### 定义：
```python
@property
def calculation_mode(self):
    ...
@calculation_mode.setter
def calculation_mode(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [CalcModeType](/cells/zh/python-net/aspose.cells/calcmodetype)
* 类 [FormulaSettings](/cells/zh/python-net/aspose.cells/formulasettings)
