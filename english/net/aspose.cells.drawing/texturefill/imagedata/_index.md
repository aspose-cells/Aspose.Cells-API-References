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
// Called: workbook.Worksheets[0].Shapes[0].Fill.TextureFill.ImageData = File.ReadAllBytes(Path.Combine(Constants.sourcePath, &amp;quot;image1.jpg&amp;quot;));
[Test]
        public void Property_ImageData()
        {
            using (Workbook workbook = new Workbook(Path.Combine(Constants.sourcePath, &quot;CellsNet44868.xls&quot;)))
            {
                //Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
                workbook.Worksheets[0].Shapes[0].Fill.FillType = FillType.Texture;
                workbook.Worksheets[0].Shapes[0].Fill.TextureFill.ImageData = File.ReadAllBytes(Path.Combine(Constants.sourcePath, &quot;image1.jpg&quot;));

                Util.SaveManCheck(workbook, &quot;Shape&quot;, &quot;CellsNet44868.xls&quot;);
            }
        }
```

### See Also

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


