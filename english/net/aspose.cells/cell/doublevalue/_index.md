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
// Called: testAreEqual(2.56, cells[65535, 0].DoubleValue, caseName);
private void Cell_Property_DoubleValue(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(1, cells[0, 0].IntValue, caseName);
            testAreEqual(true, cells[1, 0].BoolValue, caseName);
            testAreEqual("abc", cells[2, 0].StringValue, caseName);
            testAreEqual(false, cells[3, 0].BoolValue, caseName);
            testAreEqual(2.56, cells[65535, 0].DoubleValue, caseName);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


