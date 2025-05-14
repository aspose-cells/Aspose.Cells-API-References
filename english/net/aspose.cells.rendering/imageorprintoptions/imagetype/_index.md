---
title: ImageOrPrintOptions.ImageType
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the format of the generated images. default value PNG
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/imagetype/
---
## ImageOrPrintOptions.ImageType property

Gets or sets the format of the generated images. default value: PNG.

```csharp
public virtual ImageType ImageType { get; set; }
```

### Examples

```csharp
// Called: options.ImageOptions.ImageType = ImageType.Svg;
public void ImageOrPrintOptions_Property_ImageType()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41783/";
    Workbook wb = new Workbook(filePath + "工作簿3.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ImageOptions.ImageType = ImageType.Svg;
    options.ExportActiveWorksheetOnly = true;
    string savePath = CreateFolder(filePath) + "out.html";
    wb.Save(savePath, options);

    string content = File.ReadAllText(savePath);
    Assert.IsTrue(content.IndexOf(".svg") > -1);
}
```

### See Also

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


