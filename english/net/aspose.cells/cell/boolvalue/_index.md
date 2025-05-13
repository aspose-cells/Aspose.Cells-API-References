---
title: Cell.BoolValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the boolean value contained in the cell
type: docs
url: /net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Gets the boolean value contained in the cell.

```csharp
public bool BoolValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, cell.BoolValue);
public void Cell_Property_BoolValue()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    cell.Formula = "=2.01>2";
    workbook.CalculateFormula();
    Assert.AreEqual(true, cell.BoolValue);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


