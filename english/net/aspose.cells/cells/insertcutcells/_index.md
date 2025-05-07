---
title: Cells.InsertCutCells
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Insert cut range
type: docs
url: /net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Insert cut range.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cutRange | Range | The cut range. |
| row | Int32 | The row. |
| column | Int32 | The column. |
| shiftType | ShiftType | The shift type . |

### Examples

```csharp
// Called: worksheet.Cells.InsertCutCells(rowsRangeToCut, rowIndexDestination, 0, ShiftType.Down);
private static void Method_ShiftType_(Worksheet worksheet, int startRow, int endRow, int rowIndexDestination)
        {
            var usedRangeLastColumnIndex = worksheet.Cells.MaxColumn;

            var rowsRangeToCut = worksheet.Cells.CreateRange(startRow, 0, endRow - startRow + 1, 6);

            // Cut the rows and insert them above the destination row
            worksheet.Cells.InsertCutCells(rowsRangeToCut, rowIndexDestination, 0, ShiftType.Down);
        }
```

### See Also

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


