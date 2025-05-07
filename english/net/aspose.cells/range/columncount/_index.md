---
title: Range.ColumnCount
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the count of columns in the range
type: docs
url: /net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Gets the count of columns in the range.

```csharp
public int ColumnCount { get; }
```

### Examples

```csharp
// Called: cell.Column >= range.FirstColumn && cell.Column < range.FirstColumn + range.ColumnCount);
private static bool Property_ColumnCount(Cell cell, Aspose.Cells.Range range)
        {
            return (cell.Row >= range.FirstRow && cell.Row < range.FirstRow + range.RowCount &&
                cell.Column >= range.FirstColumn && cell.Column < range.FirstColumn + range.ColumnCount);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


