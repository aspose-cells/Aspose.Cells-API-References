---
title: get_dependents方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 90
url: /zh/python-net/aspose.cells/cell/get_dependents/
is_root: false
---
##  get_dependents(is_all) {#bool}
获取其公式直接引用该单元格的所有单元格。



```python
def get_dependents(self, is_all):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| is_all | bool |指示是否检查其他工作表中的公式|
### 评论

* 如果包含此单元格的引用出现在一个单元格的公式中，则该单元格将被视为

此单元格的依赖项，无论在计算时是否使用引用或此单元格。
例如，公式“=IF(TRUE,A1,A2)”中的A2单元格在计算时虽然没有使用，
这个公式仍然作为A2的依赖。
要得到那些计算结果依赖于该单元格的公式，请使用[Cell.get_dependents_in_calculation(recursive)](/cells/zh/python-net/aspose.cells/cell/get_dependents_in_calculation)。当跟踪一个单元格的依赖时，工作簿或工作表中的所有公式将被分析和检查。
所以这是一个耗时的过程。如果用户需要跟踪大量单元格的依赖项，使用此方法将
导致性能不佳。出于性能考虑，用户应改用 [Cell.get_dependents_in_calculation(recursive)](/cells/zh/python-net/aspose.cells/cell/get_dependents_in_calculation)。
或者，用户可以先通过 [Cell.get_precedents()](/cells/zh/python-net/aspose.cells/cell/get_precedents) 收集所有单元格的先例图，
然后根据先例图构建家属图。

* 如果包含此单元格的引用出现在一个单元格的公式中，则该单元格将被视为
此单元格的依赖项，无论在计算时是否使用引用或此单元格。
例如，公式“=IF(TRUE,A1,A2)”中的A2单元格在计算时虽然没有使用，
这个公式仍然作为A2的依赖。
要得到那些计算结果依赖于该单元格的公式，请使用[Cell.get_dependents_in_calculation(recursive)](/cells/zh/python-net/aspose.cells/cell/get_dependents_in_calculation)。当跟踪一个单元格的依赖时，工作簿或工作表中的所有公式将被分析和检查。
所以这是一个耗时的过程。如果用户需要跟踪大量单元格的依赖项，使用此方法将
导致性能不佳。出于性能考虑，用户应改用 [Cell.get_dependents_in_calculation(recursive)](/cells/zh/python-net/aspose.cells/cell/get_dependents_in_calculation)。
或者，用户可以先通过 [Cell.get_precedents()](/cells/zh/python-net/aspose.cells/cell/get_precedents) 收集所有单元格的先例图，
然后根据先例图构建家属图。

* 如果包含此单元格的引用出现在一个单元格的公式中，则该单元格将被视为
此单元格的依赖项，无论在计算时是否使用引用或此单元格。
例如，公式“=IF(TRUE,A1,A2)”中的A2单元格在计算时虽然没有使用，
这个公式仍然作为A2的依赖。
要得到那些计算结果依赖于该单元格的公式，请使用[Cell.get_dependents_in_calculation(recursive)](/cells/zh/python-net/aspose.cells/cell/get_dependents_in_calculation)。当跟踪一个单元格的依赖时，工作簿或工作表中的所有公式将被分析和检查。
所以这是一个耗时的过程。如果用户需要跟踪大量单元格的依赖项，使用此方法将
导致性能不佳。出于性能考虑，用户应改用 [Cell.get_dependents_in_calculation(recursive)](/cells/zh/python-net/aspose.cells/cell/get_dependents_in_calculation)。
或者，用户可以先通过 [Cell.get_precedents()](/cells/zh/python-net/aspose.cells/cell/get_precedents) 收集所有单元格的先例图，
然后根据先例图构建家属图。
### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
dependents = cells.get("B1").get_dependents(True)
for i in range(len(dependents)):
    print(dependents[i].name)

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
