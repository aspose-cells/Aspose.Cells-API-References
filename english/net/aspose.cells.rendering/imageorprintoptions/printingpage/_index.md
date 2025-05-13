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
public void ImageOrPrintOptions_Property_PrintingPage() 
{
    ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
    imgOpt.PrintingPage = PrintingPageType.IgnoreBlank;

    {
        Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
        WorkbookRender wr = new WorkbookRender(wb, imgOpt);
        Assert.AreEqual(4, wr.PageCount);
    }

    {
        Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
        WorkbookRender wr = new WorkbookRender(wb, imgOpt);
        Assert.AreEqual(2, wr.PageCount);
    }

    {
        Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
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


