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
// Called: byte[] img = bar.ToImage(cell, imgOpts);
[Test]
        public void Method_ImageOrPrintOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA44952.xlsx&quot;);
            ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
            Cell cell = workbook.Worksheets[0].Cells[&quot;C3&quot;];// mergecell, toimage only one column width.
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            if (result != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                if (bar != null)
                {
                    //  imgOpts.SetDesiredSize(600, 28);// not work
                    byte[] img = bar.ToImage(cell, imgOpts);
                    File.WriteAllBytes(Constants.destPath + &quot;CELLSJAVA44952.png&quot;, img);
                    using (Image image = Image.FromStream(new MemoryStream(img)))
                    {
                       Assert.AreEqual(602,image.Width);
                    }
                }
            }
            workbook.Save(Constants.destPath + &quot;CELLSJAVA44952.html&quot;);
        }
```

### See Also

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


