---
title: PageSetup.BottomMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the bottom margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/bottommargin/
---
## PageSetup.BottomMargin property

Represents the size of the bottom margin, in unit of centimeters.

```csharp
public double BottomMargin { get; set; }
```

### Examples

```csharp
// Called: range.Worksheet.PageSetup.BottomMargin = 0;
public void PageSetup_Property_BottomMargin()
{
    Workbook workbook = new Workbook(Constants.TemplatePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets["01_Sub_Sup_Stri"];
    Aspose.Cells.Range range = worksheet.Cells.CreateRange("B6:G20");

    range.Worksheet.PageSetup.PrintArea = range.Address;
    range.Worksheet.PageSetup.ClearHeaderFooter();
    range.Worksheet.PageSetup.LeftMargin = 0;
    range.Worksheet.PageSetup.RightMargin = 0;
    range.Worksheet.PageSetup.TopMargin = 0;
    range.Worksheet.PageSetup.BottomMargin = 0;
    range.Worksheet.PageSetup.Zoom = 100;
    ImageOrPrintOptions imageOptions = new ImageOrPrintOptions
    {
        OnePagePerSheet = true,
        ImageType = ImageType.Svg,
        SVGFitToViewPort = true
    };

    SheetRender sheetRender = new SheetRender(range.Worksheet, imageOptions);

    MemoryStream ms = new MemoryStream();
    sheetRender.ToImage(0, ms);
    ms.Seek(0, SeekOrigin.Begin);

    using (StreamReader sr = new StreamReader(ms, Encoding.UTF8))
    {
        string text = sr.ReadToEnd();
        Assert.IsTrue(text.IndexOf("text-decoration:line-through") > -1 
            || text.IndexOf("text-decoration=\"line-through\"") > -1);
    }
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


