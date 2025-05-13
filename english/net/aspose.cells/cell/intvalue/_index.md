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
// Called: Assert.AreEqual(0, cell.IntValue);
public void Cell_Property_IntValue()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Cell cell = cells[0, 1];
    cell.Formula = "=2*false";
    workbook.CalculateFormula();
    Assert.AreEqual(0, cell.IntValue);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


