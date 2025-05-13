---
title: PageSetup.PaperWidth
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Gets the width of the paper in unit of inches considered page orientation
type: docs
url: /net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

Gets the width of the paper in unit of inches, considered page orientation.

```csharp
public double PaperWidth { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(8.5, setup.PaperWidth);
public void PageSetup_Property_PaperWidth()
{
           
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].Cells["A4"].PutValue("test");
    Assert.AreEqual(1, workbook.Worksheets[0].Cells.CountLarge);
    PageSetup setup = workbook.Worksheets[0].PageSetup;
   Assert.AreEqual(11,setup.PaperHeight);
    Assert.AreEqual(8.5, setup.PaperWidth);
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


