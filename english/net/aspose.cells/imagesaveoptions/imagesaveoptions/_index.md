---
title: ImageSaveOptions.ImageSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: ImageSaveOptions constructor. Creates the options for saving image file
type: docs
url: /net/aspose.cells/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions() {#constructor}

Creates the options for saving image file.

```csharp
public ImageSaveOptions()
```

### Remarks

The default type is Tiff.

### Examples

```csharp
// Called: Aspose.Cells.ImageSaveOptions pngOptions = new Aspose.Cells.ImageSaveOptions();
public void ImageSaveOptions_Constructor()
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

* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImageSaveOptions(SaveFormat) {#constructor_1}

Creates the options for saving image file.

```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Tiff, Svg, Bmp, Png, Jpg, Emf or Gif, otherwise the saved format will be set as Tiff automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


