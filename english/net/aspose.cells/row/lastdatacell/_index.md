---
title: Row.LastDataCell
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the last nonblank cell in the row
type: docs
url: /net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Gets the last non-blank cell in the row.

```csharp
public Cell LastDataCell { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(cells.Rows[0].LastDataCell.Name, "A1");
public void Row_Property_LastDataCell()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells["A1"].PutValue("1");
    Cell cell = cells["A2"];
    Assert.AreEqual(cells.Rows[0].LastDataCell.Name, "A1");
}
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


