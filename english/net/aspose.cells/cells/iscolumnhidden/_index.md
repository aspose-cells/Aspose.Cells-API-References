---
title: Cells.IsColumnHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Checks whether a column at given index is hidden
type: docs
url: /net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Checks whether a column at given index is hidden.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | column index |

### Return Value

true if the column is hidden.

### Examples

```csharp
// Called: Assert.AreEqual(cells.IsColumnHidden(2), true);
public void Cells_Method_IsColumnHidden()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = workbook.Worksheets[0].Cells;
    Assert.AreEqual(cells.IsColumnHidden(2), true);
    Assert.AreEqual(cells.GetRowHeightPixel(1), 6);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


