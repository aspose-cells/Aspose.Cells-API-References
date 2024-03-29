---
title: SheetPrintingPreview.EvaluatedPageCount
second_title: Aspose.Cells for .NET API Reference
description: SheetPrintingPreview property. Evaluate the total page count of this worksheet
type: docs
url: /net/aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/
---
## SheetPrintingPreview.EvaluatedPageCount property

Evaluate the total page count of this worksheet

```csharp
public int EvaluatedPageCount { get; }
```

### Examples

The following code shows the fastest way to get page count of a worksheet.

```csharp
Workbook workbook = new Workbook("Book1.xlsx");

SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(workbook.Worksheets[0], new ImageOrPrintOptions());

//fastest way to get page count especailly when there are massive data in worksheet.
Console.WriteLine(sheetPrintingPreview.EvaluatedPageCount);
        
```

### See Also

* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


