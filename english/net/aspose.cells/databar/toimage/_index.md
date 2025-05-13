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
public void DataBar_Method_ToImage()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
    Cell cell = workbook.Worksheets[0].Cells["C3"];// mergecell, toimage only one column width.
    ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
    if (result != null)
    {
        DataBar bar = result.ConditionalFormattingDataBar;
        if (bar != null)
        {
            //  imgOpts.SetDesiredSize(600, 28);// not work
            byte[] img = bar.ToImage(cell, imgOpts);
            File.WriteAllBytes(Constants.destPath + "example.png", img);
            using (Image image = Image.FromStream(new MemoryStream(img)))
            {
               Assert.AreEqual(602,image.Width);
            }
        }
    }
    workbook.Save(Constants.destPath + "example.html");
}
```

### See Also

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


