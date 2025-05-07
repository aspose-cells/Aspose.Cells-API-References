---
title: Cells.MinDataColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Minimum column index of cell which contains data
type: docs
url: /net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Minimum column index of cell which contains data.

```csharp
public int MinDataColumn { get; }
```

### Remarks

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### Examples

```csharp
// Called: Assert.AreEqual(cells.MinDataColumn, 4);
[Test]
        public void Property_MinDataColumn()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET40877.xlsx");
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells.MinDataRow, 3);
            Assert.AreEqual(cells.MinDataColumn, 4);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


