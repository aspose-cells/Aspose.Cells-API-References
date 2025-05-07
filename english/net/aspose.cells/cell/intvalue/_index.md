---
title: Cell.IntValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the integer value contained in the cell
type: docs
url: /net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

Gets the integer value contained in the cell.

```csharp
public int IntValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, cell.IntValue, "Reference in list for SUM");
[Test]
        public void Property_IntValue()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(1);
            cells[0, 1].PutValue("a");
            Cell cell = cells[1, 0];
            cell.Formula = "SUM((A1,B1))";
            wb.CalculateFormula();
            Assert.AreEqual(1, cell.IntValue, "Reference in list for SUM");
            cell.Formula = "SUM(+{\"a\"})";
            wb.CalculateFormula();
            Assert.AreEqual(0, cell.IntValue, "Unary with Array for SUM");
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


