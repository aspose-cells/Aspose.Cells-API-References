---
title: WorkbookPrintingPreview.EvaluatedPageCount
second_title: Aspose.Cells for .NET API Reference
description: WorkbookPrintingPreview property. Evaluate the total page count of this workbook
type: docs
url: /net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Evaluate the total page count of this workbook

```csharp
public int EvaluatedPageCount { get; }
```

### Examples

The following code shows the fastest way to get page count of a workbook.

```csharp
Workbook workbook = new Workbook("Book1.xlsx");

WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, new ImageOrPrintOptions());

//fastest way to get page count especailly when there are massive data in workbook.
Console.WriteLine(workbookPrintingPreview.EvaluatedPageCount);
        
```

### See Also

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


