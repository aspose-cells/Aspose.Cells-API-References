---
title: PageSetup.IsPercentScale
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. If this property is False the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled
type: docs
url: /net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.

```csharp
public bool IsPercentScale { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(wb.Worksheets[0].PageSetup.IsPercentScale);
[Test]
        public void Property_IsPercentScale()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET43413/";
            HtmlLoadOptions opts = new HtmlLoadOptions(LoadFormat.Html);
            Workbook wb = new Workbook(filePath + "Template.xls", opts);
            Console.WriteLine(wb.Worksheets[0].PageSetup.Zoom);
            Console.WriteLine(wb.Worksheets[0].PageSetup.IsPercentScale);
            Assert.AreEqual(wb.Worksheets[0].PageSetup.Zoom, 80);
            Assert.AreEqual(wb.Worksheets[0].PageSetup.IsPercentScale, true);
            PdfSaveOptions so = new PdfSaveOptions();
            wb.Save(CreateFolder(filePath) + "out.xlsx");
            wb.Save(CreateFolder(filePath) + "out.pdf", so);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


