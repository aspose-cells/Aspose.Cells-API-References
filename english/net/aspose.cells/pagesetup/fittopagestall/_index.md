---
title: PageSetup.FitToPagesTall
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the number of pages tall the worksheet will be scaled to when its printed. The default value is 1
type: docs
url: /net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Represents the number of pages tall the worksheet will be scaled to when it's printed. The default value is 1.

```csharp
public int FitToPagesTall { get; set; }
```

### Remarks

You have to set FitToPagesWide as zero if you want to fit all rows on one page.

### Examples

```csharp
// Called: ps.FitToPagesTall = 1;
public void PageSetup_Property_FitToPagesTall()
{
    Workbook workbook = new Workbook();
    PageSetup ps = workbook.Worksheets[0].PageSetup;
    ps.PrintArea = "A1:G125";
    ps.FitToPagesTall = 1;
    ps.FitToPagesWide = 1;
    // ps.Zoom = 45;
    ps.PaperSize = PaperSizeType.PaperLetter;
    ps.PrintGridlines = true;
    ImageOrPrintOptions options = new ImageOrPrintOptions();
    SheetRender render = new SheetRender(workbook.Worksheets[0], options);
   Assert.AreEqual(0.41,Math.Round(render.PageScale,2));
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


