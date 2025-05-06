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
// Called: pageSetup.IsPercentScale = true;
[Test]
        public void Property_IsPercentScale()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47688/&quot;;
            string savePath = CreateFolder(filePath);

            var fileName = filePath + @&quot;f.html&quot;;
            var output2 = savePath + @&quot;out.pdf&quot;;
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            Workbook wb = new Workbook(fileName, loadOptions);
            Worksheet worksheet = wb.Worksheets[0];
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            worksheet.AutoFitRows(options);
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsPercentScale = true;
            pageSetup.Zoom = 70;
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            wb.Save(output2, saveOptions);
            wb.Save(savePath + &quot;out.xlsx&quot;);

        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


