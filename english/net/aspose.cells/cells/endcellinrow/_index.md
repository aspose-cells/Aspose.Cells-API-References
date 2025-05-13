---
title: Cells.EndCellInRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the last cell in this row
type: docs
url: /net/aspose.cells/cells/endcellinrow/
---
## EndCellInRow(int) {#endcellinrow}

Gets the last cell in this row.

```csharp
public Cell EndCellInRow(int rowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |

### Return Value

Cell object.

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EndCellInRow(int, int, int, int) {#endcellinrow_1}

Gets the last cell with maximum row index in this range.

```csharp
public Cell EndCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column index. |

### Return Value

Cell object.

### Examples

```csharp
// Called: Cell objCell = objWS.Cells.EndCellInRow(0, 14, 0, 4);//exception
public void Cells_Method_EndCellInRow()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet objWS = workbook.Worksheets[0];

    Cell objCell = objWS.Cells.EndCellInRow(0, 14, 0, 4);//exception
}
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


