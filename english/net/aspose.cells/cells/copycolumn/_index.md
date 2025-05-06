---
title: Cells.CopyColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of a whole column
type: docs
url: /net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Copies data and formats of a whole column.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| destinationColumnIndex | Int32 | Destination column index. |

### Examples

```csharp
// Called: destCells.CopyColumn(srcCells, -1, 2);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = &quot;testCopyColumn_Exception_001&quot;;
            Workbook workbook = new Workbook();
            Cells srcCells = workbook.Worksheets[0].Cells;
            Cells destCells = workbook.Worksheets[workbook.Worksheets.Add()].Cells;
            destCells.CopyColumn(srcCells, -1, 2);
            string msg = message + &quot;destCells.CopyColumn(srcCells, -1, 2)&quot;;
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


