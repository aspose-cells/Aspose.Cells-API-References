---
title: Cells.CheckCell
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the Cell element or null at the specified cell row index and column index
type: docs
url: /net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Gets the [`Cell`](../../cell/) element or null at the specified cell row index and column index.

```csharp
public Cell CheckCell(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
| column | Int32 | Column index |

### Return Value

Return Cell object if a Cell object exists. Return null if the cell does not exist.

### Examples

```csharp
// Called: Cell cell = cells.CheckCell(row, col);
public static void Method_Int32_(Cells cells, int row, int col, string msg)
        {
            Cell cell = cells.CheckCell(row, col);
            if (cell == null)
            {
                Assert.Fail(msg + " should not be empty cell");
            }
            if (cell.IsNumericValue)
            {
                return;
            }
            if (cell.Type == CellValueType.IsNull)
            {
                Assert.Fail(msg + " should not be empty cell");
            }
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


