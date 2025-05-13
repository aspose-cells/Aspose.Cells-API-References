---
title: Cell.IsFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents if the specified cell contains formula
type: docs
url: /net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Represents if the specified cell contains formula.

```csharp
public bool IsFormula { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[8].Cells["F47"].IsFormula);
public void Cell_Property_IsFormula()
{

    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.IsTrue(workbook.Worksheets[8].Cells["F47"].IsFormula);
    Shape shape = workbook.Worksheets[0].Shapes[8];
    shape.Text = ("Hello world!");
    Assert.IsTrue(workbook.Worksheets[8].Cells["F47"].IsFormula);

}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


