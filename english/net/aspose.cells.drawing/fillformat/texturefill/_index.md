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
public void FillFormat_Property_TextureFill()
{
    var wb = new Workbook(Constants.sourcePath + "example.xlsx");

    Picture pictureShape = (Picture)wb.Worksheets[0].Shapes[0];

    // Background and foreground images are not equal, but Aspose.Cells returns same data.
    Assert.IsFalse(pictureShape.Fill.TextureFill.ImageData == pictureShape.Data);

    // This line properly changes the foreground image, but the background image is also changed.
    pictureShape.Data = File.ReadAllBytes(Path.Combine(Constants.sourcePath, "image1.png"));



    wb.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.destPath + "example.xlsx");
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


