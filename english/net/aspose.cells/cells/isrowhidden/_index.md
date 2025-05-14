---
title: Cells.IsRowHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Checks whether a row at given index is hidden
type: docs
url: /net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Checks whether a row at given index is hidden.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | row index |

### Return Value

true if the row is hidden

### Examples

```csharp
// Called: Assert.AreEqual(i != 3 && i != 5, cells.IsRowHidden(i), "Row-" + i + ".Hidden");
public void Cells_Method_IsRowHidden()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Cells cells = sheet.Cells;
    cells[1, 0].PutValue("US");
    cells[2, 0].PutValue("UK");
    cells[3, 0].PutValue("India");
    cells[4, 0].PutValue("UK");
    cells[5, 0].PutValue("India");
    cells[6, 0].PutValue("US");
    for (int i = 1; i < 10; i++)
    {
        cells[i, 1].PutValue(i);
    }
    AutoFilter af = sheet.AutoFilter;
    af.Range = "A1:A1";
    af.Filter(0, "India");
    af.Refresh();
    for (int i = 1; i < 10; i++)
    {
        Assert.AreEqual(i != 3 && i != 5, cells.IsRowHidden(i), "Row-" + i + ".Hidden");
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


