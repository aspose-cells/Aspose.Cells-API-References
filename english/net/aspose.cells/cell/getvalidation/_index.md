---
title: Cell.GetValidation
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the validation applied to this cell
type: docs
url: /net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Gets the validation applied to this cell.

```csharp
public Validation GetValidation()
```

### Examples

```csharp
// Called: Assert.AreEqual(ValidationType.AnyValue, cell.GetValidation().Type);
public void Cell_Method_GetValidation()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Cell cell = wb.Worksheets[0].Cells["B11"];
    Assert.AreEqual(ValidationType.AnyValue, cell.GetValidation().Type);
}
```

### See Also

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


