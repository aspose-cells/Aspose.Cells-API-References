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
// Called: Assert.AreEqual(-295495.5684, cells[0, 0].DoubleValue, 0.0001);
[Test]
      public void Property_DoubleValue()
      {
          Workbook workbook = new Workbook();
          Cells cells = workbook.Worksheets[0].Cells;
          cells[0, 0].Formula = "=FV(8%/12,12*20,500,200)";
          workbook.CalculateFormula();
          Assert.AreEqual(-295495.5684, cells[0, 0].DoubleValue, 0.0001);
      }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


