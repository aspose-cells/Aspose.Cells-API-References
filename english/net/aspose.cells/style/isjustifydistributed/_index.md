---
title: Style.IsJustifyDistributed
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates if the cells justified or distributed alignment should be used on the last line of text
type: docs
url: /net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Indicates if the cells justified or distributed alignment should be used on the last line of text.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Remarks

This is typical for East Asian alignments but not typical in other contexts.

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Cells["B3"].GetStyle().IsJustifyDistributed);
public void Style_Property_IsJustifyDistributed()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.IsTrue(workbook.Worksheets[0].Cells["B3"].GetStyle().IsJustifyDistributed);
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


