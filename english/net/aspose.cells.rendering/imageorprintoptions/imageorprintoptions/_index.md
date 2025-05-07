---
title: ImageOrPrintOptions.ImageOrPrintOptions
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions constructor. Ctor
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/imageorprintoptions/
---
## ImageOrPrintOptions constructor

Ctor.

```csharp
public ImageOrPrintOptions()
```

### Examples

```csharp
// Called: ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
[Test]
        public void ImageOrPrintOptions_Constructor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "21010_2003.xls");
            Worksheet sheet = workbook.Worksheets[0];
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
            imgOptions.ImageType = ImageType.Jpeg;
            SheetRender sheetRender = new SheetRender(sheet, imgOptions);
            Bitmap bitmap = sheetRender.ToImage(0);
            bitmap.Save(Constants.destPath + "21010_2003.jpg", ImageFormat.Jpeg);
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


