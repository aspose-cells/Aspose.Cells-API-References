---
title: DataBar.ToImage
second_title: Aspose.Cells for .NET API Reference
description: DataBar method. Render data bar in cell to image byte array
type: docs
url: /net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

Render data bar in cell to image byte array.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Indicate the data bar in which cell to be rendered |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |

### Examples

```csharp
// Called: byte[] data = dataBar.ToImage(cell, imgOpts);
[Test]
        public void Method_ImageOrPrintOptions_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "ConditionalFormattings/CELLSJAVA-43689.xlsx");
            Worksheet worksheet = wb.Worksheets[0];
            Cell cell = worksheet.Cells["G7"];
            DataBar dataBar = cell.GetConditionalFormattingResult().ConditionalFormattingDataBar;
            ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
            imgOpts.ImageType = ImageType.Png;
            byte[] data = dataBar.ToImage(cell, imgOpts);

            using(Bitmap b = (Bitmap)Image.FromStream(new MemoryStream(data)))
            {
                Color color = b.GetPixel(10, 10);
                Assert.AreEqual(255, color.R);
            }
        }
```

### See Also

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


