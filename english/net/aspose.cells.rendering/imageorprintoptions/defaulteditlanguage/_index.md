---
title: ImageOrPrintOptions.DefaultEditLanguage
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets default edit language
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/
---
## ImageOrPrintOptions.DefaultEditLanguage property

Gets or sets default edit language.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Remarks

It may display/render different layouts for text paragraph when different edit languages is set. Default is Auto.

### Examples

```csharp
// Called: imageOrPrintOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
public void ImageOrPrintOptions_Property_DefaultEditLanguage()
{
    Workbook wb = new Workbook(Constants.TemplatePath + "example.xlsx");

    ImageOrPrintOptions imageOrPrintOptions = new ImageOrPrintOptions();
    imageOrPrintOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
    imageOrPrintOptions.ImageType = ImageType.Png;
    SheetRender sr = new SheetRender(wb.Worksheets["Sheet1"], imageOrPrintOptions);

    MemoryStream ms = new MemoryStream();
    sr.ToImage(0, ms);
    ms.Position = 0;

    Bitmap expectedImage = (Bitmap)Image.FromFile(Constants.TemplatePath + "example.png");
    Bitmap generatedImage = (Bitmap)Image.FromStream(ms);

    int diffCount = ImageCompareUtil.CompareImage(expectedImage, generatedImage);

    Assert.Less(diffCount, 10);

}
```

### See Also

* enum [DefaultEditLanguage](../../../aspose.cells/defaulteditlanguage/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


