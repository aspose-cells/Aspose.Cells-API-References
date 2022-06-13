---
title: VerticalPageBreak
second_title: Aspose.Cells for .NET API 参考
description: 封装表示垂直分页符的对象
type: docs
weight: 6310
url: /zh/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

封装表示垂直分页符的对象。

```csharp
public class VerticalPageBreak
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column) { get; } | 获取垂直分页符的列索引。 |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow) { get; } | 获取垂直分页符的结束行索引。 |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow) { get; } | 获取垂直分页符的起始行索引。 |

### 例子

```csharp
[C#]
Workbook excel = new Workbook();
 //在G5

excel.Worksheets[0].HorizontalPageBreaks.Add("G5");
excel.Worksheets[0].VerticalPageBreaks.Add("G5");

[VB]
Dim excel as Workbook = new Workbook()
'Add a pagebreak at G5
excel.Worksheets(0).HorizontalPageBreaks.Add("G5")
excel.Worksheets(0).VerticalPageBreaks.Add("G5")
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->