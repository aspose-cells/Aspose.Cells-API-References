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
// Called: imgOptions.ImageType = ImageType.Svg;
[Test]
        public void Property_ImageType()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43077/";

            Workbook wb = new Workbook(filePath + "DataAndChart.xlsx");

            wb.Worksheets.ActiveSheetIndex = 0;
            // export the worksheet
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            options.Encoding = Encoding.UTF8;
            options.PresentationPreference = true;
            options.ExportActiveWorksheetOnly = true;
            options.ExportImagesAsBase64 = true;


            // *tries* to set the Chart Shape to SVG@ 300DPI, but results in PNG
            ImageOrPrintOptions imgOptions = options.ImageOptions;
            imgOptions.ImageType = ImageType.Svg;
            imgOptions.HorizontalResolution = 300;
            imgOptions.VerticalResolution = 300;

            wb.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


