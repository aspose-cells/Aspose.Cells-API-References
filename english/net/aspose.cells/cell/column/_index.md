---
title: Cell.Column
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets column number zero based of the cell
type: docs
url: /net/aspose.cells/cell/column/
---
## Cell.Column property

Gets column number (zero based) of the cell.

```csharp
public int Column { get; }
```

### Examples

```csharp
// Called: CellArea expected = CellArea.CreateCellArea(cell.Row, cell.Column, cell.Row, cell.Column);
[Test]
        public void Property_Column()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            string[] data = new string[]
            {
                "A2", "=ABS(B:B)",
                "C1", "=2:3",
                "A1048570", "=A1:A10",
                "XFA1", "=A2:H2",
            };
            for (int i = 0; i < data.Length; i += 2)
            {
                Cell cell = cells[data[i]];
                string fml = data[i + 1];
                CellArea ca = cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
                CellArea expected = CellArea.CreateCellArea(cell.Row, cell.Column, cell.Row, cell.Column);
                CheckArrayFormula(fml, cells, expected, "");
                Assert.AreEqual("#VALUE!", cell.Value, fml + " for " + data[i] + " should produce SPILLERR");
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


