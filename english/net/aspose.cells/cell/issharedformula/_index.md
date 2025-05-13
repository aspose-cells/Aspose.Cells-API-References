---
title: Cell.IsSharedFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the cell formula is part of shared formula
type: docs
url: /net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Indicates whether the cell formula is part of shared formula.

```csharp
public bool IsSharedFormula { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(cell.IsSharedFormula);
public void Cell_Property_IsSharedFormula()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ApplyFormulas(workbook, workbook.Worksheets[2]);
    Cell cell = workbook.Worksheets[2].Cells["D3"];
    Assert.IsFalse(cell.IsSharedFormula);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


