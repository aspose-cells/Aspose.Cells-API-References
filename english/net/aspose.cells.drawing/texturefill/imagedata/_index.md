---
title: TextureFill.ImageData
second_title: Aspose.Cells for .NET API Reference
description: TextureFill property. Gets and sets the image data of the fill
type: docs
url: /net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

Gets and sets the image data of the fill.

```csharp
public byte[] ImageData { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(pictureShape.Fill.TextureFill.ImageData == pictureShape.Data);
[Test]
        public void Property_ImageData()
        {
            var wb = new Workbook(Constants.sourcePath + "CellsNet45774.xlsx");

            Picture pictureShape = (Picture)wb.Worksheets[0].Shapes[0];

            // Background and foreground images are not equal, but Aspose.Cells returns same data.
            Assert.IsFalse(pictureShape.Fill.TextureFill.ImageData == pictureShape.Data);

            // This line properly changes the foreground image, but the background image is also changed.
            pictureShape.Data = File.ReadAllBytes(Path.Combine(Constants.sourcePath, "image1.png"));



            wb.Save(Constants.destPath + "CellsNet45774.xlsx");
            wb = new Workbook(Constants.destPath + "CellsNet45774.xlsx");
            pictureShape = (Picture)wb.Worksheets[0].Shapes[0];

            // Background and foreground images are not equal, but Aspose.Cells returns same data.
            Assert.IsFalse(pictureShape.Fill.TextureFill.ImageData == pictureShape.Data);
        }
```

### See Also

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


