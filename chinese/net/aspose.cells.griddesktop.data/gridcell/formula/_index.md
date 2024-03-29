---
title: Formula
second_title: Aspose.Cells for .NET API 参考
description: 获取或设置公式Cell.
type: docs
weight: 70
url: /zh/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

获取或设置公式Cell.

```csharp
public string Formula { get; set; }
```

### 评论

公式字符串始终以等号 (=) 开头。 并且请始终使用逗号 (,) 作为参数分隔符，例如“=SUM(A1, E1, H2)”。

用户可以在工作簿设计器文件中设置任何公式。 Aspose.Cells 将保留所有公式。 如果用户使用此属性为单元格设置公式，则支持 Workbook 内置函数的主要部分 。还有更多即将到来。如果您对 Workbook 内置功能有任何特殊需求， 请告诉我们。

### 例子

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### 也可以看看

* class [GridCell](../../gridcell)
* 命名空间 [Aspose.Cells.GridDesktop.Data](../../gridcell)
* 部件 [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
