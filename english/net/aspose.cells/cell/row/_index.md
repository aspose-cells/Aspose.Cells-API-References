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
// Called: testAreEqual(1, cell.Row, caseName);
private void Cell_Property_Row(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells.Find("=SUM(A1", null, new FindOptions()
            { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
            testAreEqual(1, cell.Row, caseName);
            testAreEqual(1, cell.Column, caseName);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


