---
title: Worksheet.IsPageBreakPreview
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether the specified worksheet is shown in normal view or page break preview
type: docs
url: /net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

Indicates whether the specified worksheet is shown in normal view or page break preview.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].IsPageBreakPreview, true);
public void Worksheet_Property_IsPageBreakPreview()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(workbook.Worksheets[0].IsPageBreakPreview, true);
    Assert.AreEqual(workbook.Worksheets[0].Zoom, 100);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


