---
title: get_precedents_in_calculation方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 190
url: /zh/python-net/aspose.cells/cell/get_precedents_in_calculation/
is_root: false
---
##  get_precedents_in_calculation() {#}
获取此单元格公式在计算时使用的所有先例（引用当前工作簿中的单元格）。


### 返回

枚举器枚举所有引用（ReferredArea）


```python
def get_precedents_in_calculation(self):
    ...
```


### 评论

此方法只适用于[FormulaSettings.enable_calculation_chain](/cells/zh/python-net/aspose.cells/formulasettings#enable_calculation_chain)的情况
对于工作簿为真，并且工作簿已完全计算。
如果此单元格不是公式或未引用任何其他单元格，则返回 null。
### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("A2").get_precedents_in_calculation()
print("A2's calculation precedents:")
for r in en:
    print(r)

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
