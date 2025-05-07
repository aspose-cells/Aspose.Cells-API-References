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
// Called: PrintingPage = PrintingPageType.IgnoreBlank,
[Test]
        public void Property_PrintingPage()
        {
            var workbook = new Workbook();
            workbook.Worksheets[0].PageSetup.PrintArea = "A1:A1";
            workbook.Worksheets[0].Cells["A1"].PutValue("");
            var test = workbook.Worksheets[0].Cells["A1"].Characters(0, 0);


            var opt = new ImageOrPrintOptions
            {
                PrintingPage = PrintingPageType.IgnoreBlank,
                //ImageFormat = ImageFormat.Png,
                ImageType = ImageType.Png,
                OnePagePerSheet = true,
                OnlyArea = true
            };
            var sh1 = new SheetRender(workbook.Worksheets[0], opt);
#if !NETCOREAPP2_0
            var image = sh1.ToImage(0);
#else
            sh1.ToImage(0, Constants.destPath + "CELLSNET46207.png");
#endif
        }
```

### See Also

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


