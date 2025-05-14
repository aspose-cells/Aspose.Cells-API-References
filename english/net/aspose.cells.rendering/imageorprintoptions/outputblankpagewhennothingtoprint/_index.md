---
title: ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Indicates whether to output a blank page when there is nothing to print
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Indicates whether to output a blank page when there is nothing to print.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Remarks

Default is false.

### Examples

```csharp
// Called: imgOpts.OutputBlankPageWhenNothingToPrint = true;
public void ImageOrPrintOptions_Property_OutputBlankPageWhenNothingToPrint()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");

    ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
    imgOpts.ImageType = ImageType.Png;
    imgOpts.OnePagePerSheet = true;
    imgOpts.OutputBlankPageWhenNothingToPrint = true;

    SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpts);
    Assert.AreEqual(1, sr.PageCount);
            
    MemoryStream ms = new MemoryStream();
    sr.ToImage(0, ms);
    Assert.IsTrue(ms.ToArray().Length > 0);
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


