---
title: get_dependents_in_calculation方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells/cell/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(recursive) {#bool}
获取计算结果依赖于此单元格的所有单元格。


### 返回

枚举器枚举所有依赖项（Cell 对象）


```python
def get_dependents_in_calculation(self, recursive):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| recursive | bool |是否返回那些不直接引用此单元格的依赖项<br/>但引用此单元格的其他叶子|
### 评论

要使用此方法，请确保工作簿已设置为真值
[FormulaSettings.enable_calculation_chain](/cells/zh/python-net/aspose.cells/formulasettings#enable_calculation_chain) 并已使用此设置进行了全面计算。
如果没有对该单元格的公式引用，将返回 null。
### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("B1").get_dependents_in_calculation(False)
print("B1's calculation dependents:")
for c in en:
    print(c.name)
en = cells.get("B2").get_dependents_in_calculation(False)
print("B2's calculation dependents:")
for c in en:
    print(c.name)

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
