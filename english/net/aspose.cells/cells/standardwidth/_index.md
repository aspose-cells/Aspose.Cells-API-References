---
title: Cells.StandardWidth
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default column width in the worksheet in unit of characters
type: docs
url: /net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Gets or sets the default column width in the worksheet, in unit of characters.

```csharp
public double StandardWidth { get; set; }
```

### Examples

```csharp
// Called: cells.StandardWidth = 18.25;
public void Cells_Property_StandardWidth()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells.ApplyStyle(wb.CreateStyle(), new StyleFlag());
    cells.StandardWidth = 18.25;
    Assert.AreEqual(0, cells.Columns.Count, "Count of customed columns");
    if (cells.GetColumnWidth(0) < 17.0)
    {
        Assert.Fail("Default column width should be about 18.25");
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


