---
title: Worksheet.DisplayRightToLeft
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false
type: docs
url: /net/aspose.cells/worksheet/displayrighttoleft/
---
## Worksheet.DisplayRightToLeft property

Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false.

```csharp
public bool DisplayRightToLeft { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].DisplayRightToLeft);
public void Worksheet_Property_DisplayRightToLeft()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    Assert.IsTrue(workbook.Worksheets[0].DisplayRightToLeft);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Assert.IsTrue(workbook.Worksheets[0].DisplayRightToLeft);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


