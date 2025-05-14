---
title: Cells.HideColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Hides a column
type: docs
url: /net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Hides a column.

```csharp
public void HideColumn(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |

### Examples

```csharp
// Called: cells.HideColumn(2);
public void Cells_Method_HideColumn()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells.HideColumn(2);
    cells.UnhideColumn(2, -1);
    Assert.AreEqual(cells.Columns[2].Width, cells.StandardWidth);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


