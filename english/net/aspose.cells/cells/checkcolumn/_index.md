---
title: Cells.CheckColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the Column element or null at the specified column index
type: docs
url: /net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

Gets the [`Column`](../../column/) element or null at the specified column index.

```csharp
public Column CheckColumn(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | The column index. |

### Return Value

The Column object.

### Examples

```csharp
// Called: Assert.IsNotNull(cells.CheckColumn(4));
public void Cells_Method_CheckColumn()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells["B3"].PutValue("4");
    cells.Columns[4].IsHidden = true;
    Assert.IsNotNull(cells.CheckColumn(4));
    Assert.IsNotNull(cells.CheckRow(2));
}
```

### See Also

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


