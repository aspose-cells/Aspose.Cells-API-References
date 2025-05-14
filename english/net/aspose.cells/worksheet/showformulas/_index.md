---
title: Worksheet.ShowFormulas
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether to show formulas or their results
type: docs
url: /net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Indicates whether to show formulas or their results.

```csharp
public bool ShowFormulas { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets[0].ShowFormulas = true;
public void Worksheet_Property_ShowFormulas()
{
    Workbook wb = new Workbook();
    wb.Worksheets[0].ShowFormulas = true;
    Cell cell = wb.Worksheets[0].Cells[0, 0];
    cell.PutValue(890.93485984659992);
    Assert.AreEqual("890.9348598466", cell.DisplayStringValue);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


