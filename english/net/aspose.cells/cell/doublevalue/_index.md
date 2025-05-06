---
title: Cell.DoubleValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the double value contained in the cell
type: docs
url: /net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

Gets the double value contained in the cell.

```csharp
public double DoubleValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(-1, cells[0, 0].DoubleValue);
[Test]
      public void Property_DoubleValue()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].Formula = &quot;=MOD(-3, -2)&quot;;
            workbook.CalculateFormula();
            Assert.AreEqual(-1, cells[0, 0].DoubleValue);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


