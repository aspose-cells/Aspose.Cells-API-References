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
// Called: chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
public void TextureFill_Property_ImageData()
{
    using (Workbook workbook = new Workbook(Path.Combine(Constants.sourcePath, "example.xlsx")))
    {
        var worksheet = workbook.Worksheets[0];
        var imageData = File.ReadAllBytes(Path.Combine(Constants.sourcePath, "example.png"));
        foreach (Chart chart in worksheet.Charts)
        {
            if (chart.ChartArea.Area.FillFormat.FillType == FillType.Texture)
            {
                chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            }
        }
        Util.SaveManCheck(workbook, "Shape", "example.xlsx");
    }
}
```

### See Also

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


