---
title: PageSetup.FitToPagesWide
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the number of pages wide the worksheet will be scaled to when its printed. The default value is 1
type: docs
url: /net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Represents the number of pages wide the worksheet will be scaled to when it's printed. The default value is 1.

```csharp
public int FitToPagesWide { get; set; }
```

### Remarks

You have to set FitToPagesTall as zero if you want to fit all columns on one page.

### Examples

```csharp
// Called: ps.FitToPagesWide = 1;
[Test]
        public void Property_FitToPagesWide()
        {
            Workbook workbook = new Workbook();
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            ps.PrintArea = &quot;A1:G125&quot;;
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


