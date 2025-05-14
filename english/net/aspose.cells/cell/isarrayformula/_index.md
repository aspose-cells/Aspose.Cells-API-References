---
title: Cell.IsArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the cell formula is an array formula
type: docs
url: /net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Indicates whether the cell formula is an array formula.

```csharp
public bool IsArrayFormula { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[1].Cells["B2"].IsArrayFormula, true);
public void Cell_Property_IsArrayFormula()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets[1].ListObjects[0].AutoFilter.Sorter.Sort();
    Assert.AreEqual(workbook.Worksheets[1].Cells["B2"].IsArrayFormula, true);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


