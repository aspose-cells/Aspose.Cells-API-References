---
title: Cells.MaxColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum column index of those cells that have been instantiated in the collectiondoes not include the column where style is defined for the whole column but no cell has been instantiated in it
type: docs
url: /net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

```csharp
public int MaxColumn { get; }
```

### Remarks

Return -1 if there is no cell has been instantiated.

### Examples

```csharp
// Called: int maxColumn = cells.MaxColumn;
private static void Property_MaxColumn(Worksheet wk)
        {
            Cells cells = wk.Cells;
            int maxColumn = cells.MaxColumn;
            int maxRow = cells.MaxRow;
            // PrepareNewRows(cells, maxRow, maxColumn);
            PrepareNewRows(cells, maxRow + 1, maxColumn, "Count", "=COUNT(M2:M" + maxRow.ToString() + ")");
            PrepareNewRows(cells, maxRow + 2, maxColumn, "25th Percentile", "=PERCENTILE.INC(M2:M" + maxRow.ToString() + ", .25)");
            PrepareNewRows(cells, maxRow + 3, maxColumn, "Mean", "=PERCENTILE.INC(M2:M" + maxRow.ToString() + ", .50)");
            PrepareNewRows(cells, maxRow + 4, maxColumn, "Median", "=MEDIAN(M2:M" + maxRow.ToString() + ")");
            PrepareNewRows(cells, maxRow + 5, maxColumn, "75th Percentile", "=PERCENTILE.INC(M2:M" + maxRow.ToString() + ", .75)");
            PrepareNewRows(cells, maxRow + 6, maxColumn, "90th Percentile", "=PERCENTILE.INC(M2:M" + maxRow.ToString() + ", .90)");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


