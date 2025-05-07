---
title: Cell.Row
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets row number zero based of the cell
type: docs
url: /net/aspose.cells/cell/row/
---
## Cell.Row property

Gets row number (zero based) of the cell.

```csharp
public int Row { get; }
```

### Property Value

Cell row number

### Examples

```csharp
// Called: testAreEqual(2, cell.Row, caseName);
private void Property_Row(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            CellArea cellarea = common.setCellArea(1, 1, 3, 3);
            Cell previousCell = cells[2, 1];
            rangeOptions.SetRange(cellarea);

            rangeOptions.SearchBackward = false;
            Cell cell = cells.Find("abc", previousCell, rangeOptions);
            testAreEqual(2, cell.Row, caseName);
            testAreEqual(2, cell.Column, caseName);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


