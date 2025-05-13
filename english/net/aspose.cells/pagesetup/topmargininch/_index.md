---
title: PageSetup.TopMarginInch
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the top margin in unit of inches
type: docs
url: /net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

Represents the size of the top margin, in unit of inches.

```csharp
public double TopMarginInch { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0.75, sheet.PageSetup.TopMarginInch);
public void PageSetup_Property_TopMarginInch()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet = workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex];
    Assert.AreEqual(0.75, sheet.PageSetup.TopMarginInch);
    workbook.Save(Constants.destPath + "example.jpg");
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


