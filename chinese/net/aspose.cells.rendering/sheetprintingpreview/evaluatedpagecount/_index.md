---
title: EvaluatedPageCount
second_title: Aspose.Cells for .NET API 参考
description: 评估此工作表的总页数
type: docs
weight: 20
url: /zh/net/aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/
---
## SheetPrintingPreview.EvaluatedPageCount property

评估此工作表的总页数

```csharp
public int EvaluatedPageCount { get; }
```

### 例子

以下代码显示了获取工作表页数的最快方法。

```csharp
Workbook workbook = new Workbook("Book1.xlsx");

SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(workbook.Worksheets[0], new ImageOrPrintOptions());

//当工作表中有大量数据时，获取页数的最快方法。
Console.WriteLine(sheetPrintingPreview.EvaluatedPageCount);
        
```

### 也可以看看

* class [SheetPrintingPreview](../../sheetprintingpreview)
* 命名空间 [Aspose.Cells.Rendering](../../sheetprintingpreview)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
