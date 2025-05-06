---
title: ImageOrPrintOptions.PrintingPage
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Indicates which pages will not be printed
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/printingpage/
---
## ImageOrPrintOptions.PrintingPage property

Indicates which pages will not be printed.

```csharp
public PrintingPageType PrintingPage { get; set; }
```

### Examples

```csharp
// Called: imgOpt.PrintingPage = PrintingPageType.IgnoreBlank;
[Test]
        public void Property_PrintingPage() 
        {
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.PrintingPage = PrintingPageType.IgnoreBlank;

            {
                Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45252/log_scale_test_1-_crashes_system.xlsx&quot;);
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(4, wr.PageCount);
            }

            {
                Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45252/Chart.xlsx&quot;);
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(2, wr.PageCount);
            }

            {
                Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-45252/Calibri2.xlsx&quot;);
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(3, wr.PageCount);
            }
        }
```

### See Also

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


