---
title: Cell.FloatValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the float value contained in the cell
type: docs
url: /net/aspose.cells/cell/floatvalue/
---
## Cell.FloatValue property

Gets the float value contained in the cell.

```csharp
public float FloatValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(grid.Cells[12, 2].FloatValue, 1);
[Test, Category("Bug")]
        public void Cell_Property_FloatValue()
        {
            Workbook workbook = new Workbook();
            Worksheet grid = workbook.Worksheets[0];
            Aspose.Cells.Cell cell = grid.Cells[0, 2];
            cell.Formula = "=3-2";
            grid.Workbook.CalculateFormula(false);
            cell.SetSharedFormula(cell.Formula, 13, 1);
            grid.Workbook.CalculateFormula(false);
            Assert.AreEqual(grid.Cells[12, 2].FloatValue, 1);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


