---
title: PageSetup.IsAutomaticPaperSize
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Indicates whether the paper size is automatic
type: docs
url: /net/aspose.cells/pagesetup/isautomaticpapersize/
---
## PageSetup.IsAutomaticPaperSize property

Indicates whether the paper size is automatic.

```csharp
public bool IsAutomaticPaperSize { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(ps.IsAutomaticPaperSize);
public void PageSetup_Property_IsAutomaticPaperSize()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    PageSetup ps = workbook.Worksheets[0].PageSetup;
    Assert.IsFalse(ps.IsAutomaticPaperSize);
    ps = workbook.Worksheets[3].PageSetup;
    Assert.IsTrue(ps.IsAutomaticPaperSize);
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


