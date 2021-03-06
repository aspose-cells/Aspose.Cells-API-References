---
title: GetDependentsInCalculation
second_title: Aspose.Cells for .NET API 参考
description: 获取计算结果依赖于该单元格的所有单元格
type: docs
weight: 390
url: /zh/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

获取计算结果依赖于该单元格的所有单元格。

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| recursive | Boolean | 是否返回那些不直接引用此单元格的依赖项 但引用其他叶子此单元格 |

### 返回值

枚举器枚举所有依赖项（单元格）

### 评论

This方法仅适用于[`EnableCalculationChain`](../../formulasettings/enablecalculationchain) 对于工作簿为真且工作簿已被完全计算的情况。 如果没有对该单元格的公式引用，则返回 null。

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
IEnumerator en = cells["B1"].GetDependentsInCalculation();
while(en.MoveNext())
{
     Console.WriteLine(((Cell)en.Current).Name);
}
```

### 也可以看看

* class [Cell](../../cell)
* 命名空间 [Aspose.Cells](../../cell)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
