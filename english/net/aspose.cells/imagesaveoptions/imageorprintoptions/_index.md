---
title: ImageSaveOptions.ImageOrPrintOptions
second_title: Aspose.Cells for .NET API Reference
description: ImageSaveOptions property. Additional image creation options
type: docs
url: /net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Additional image creation options.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Remarks

For advanced usage, please use [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) or [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Examples

```csharp
// Called: pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;
public void ImageSaveOptions_Property_ImageOrPrintOptions()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].Cells["A1"].PutValue("sdfsdf");
    Aspose.Cells.ImageSaveOptions pngOptions = new Aspose.Cells.ImageSaveOptions();
    pngOptions.ImageOrPrintOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
    pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
    pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;
    MemoryStream ms = new MemoryStream();
    workbook.Save(ms, pngOptions);
    byte x = ms.GetBuffer()[0];
    Assert.AreEqual(0x89, x);
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


