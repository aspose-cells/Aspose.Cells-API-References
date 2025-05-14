---
title: Worksheet.FirstVisibleColumn
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents first visible column index
type: docs
url: /net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Represents first visible column index.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, workbook.Worksheets[0].FirstVisibleColumn);
public void Worksheet_Property_FirstVisibleColumn()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells.HideColumn(0);
    cells.HideRow(0);
    Assert.AreEqual(1, workbook.Worksheets[0].FirstVisibleRow);
    Assert.AreEqual(1, workbook.Worksheets[0].FirstVisibleColumn);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


