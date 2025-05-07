---
title: ImageOrPrintOptions.Transparent
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Indicates if the background of generated image should be transparent
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

Indicates if the background of generated image should be transparent.

```csharp
public bool Transparent { get; set; }
```

### Remarks

The default value is false. That means the background of the generated images is white.

### Examples

```csharp
// Called: options.ImageOptions.Transparent = true;
[Test]
        public void Property_Transparent()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42204/";
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = ImageType.Png;
            options.ExportImagesAsBase64 = true;
            options.ImageOptions.Transparent = true;
            options.ExportActiveWorksheetOnly = true;

            Workbook book = new Workbook(filePath + "so-copy.xls");
            book.CalculateFormula();
            book.Worksheets.ActiveSheetIndex = 1;
            book.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


