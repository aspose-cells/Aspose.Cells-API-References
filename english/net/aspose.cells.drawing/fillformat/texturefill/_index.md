---
title: FillFormat.TextureFill
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets TextureFill object
type: docs
url: /net/aspose.cells.drawing/fillformat/texturefill/
---
## FillFormat.TextureFill property

Gets `TextureFill` object.

```csharp
public TextureFill TextureFill { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(pictureShape.Fill.TextureFill.ImageData == pictureShape.Data);
[Test]
        public void Property_TextureFill()
        {
            var wb = new Workbook(Constants.sourcePath + &quot;CellsNet45774.xlsx&quot;);

            Picture pictureShape = (Picture)wb.Worksheets[0].Shapes[0];

            // Background and foreground images are not equal, but Aspose.Cells returns same data.
            Assert.IsFalse(pictureShape.Fill.TextureFill.ImageData == pictureShape.Data);

            // This line properly changes the foreground image, but the background image is also changed.
            pictureShape.Data = File.ReadAllBytes(Path.Combine(Constants.sourcePath, &quot;image1.png&quot;));



            wb.Save(Constants.destPath + &quot;CellsNet45774.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CellsNet45774.xlsx&quot;);
            pictureShape = (Picture)wb.Worksheets[0].Shapes[0];

            // Background and foreground images are not equal, but Aspose.Cells returns same data.
            Assert.IsFalse(pictureShape.Fill.TextureFill.ImageData == pictureShape.Data);
        }
```

### See Also

* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


