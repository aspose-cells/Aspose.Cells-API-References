---
title: TextureFill.TilePicOption
second_title: Aspose.Cells for .NET API Reference
description: TextureFill property. Gets or sets tile picture option
type: docs
url: /net/aspose.cells.drawing/texturefill/tilepicoption/
---
## TextureFill.TilePicOption property

Gets or sets tile picture option.

```csharp
public TilePicOption TilePicOption { get; set; }
```

### Examples

```csharp
// Called: chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
public void TextureFill_Property_TilePicOption()
{
    using (Workbook workbook = new Workbook(Path.Combine(Constants.sourcePath, "example.xls")))
    {
        var imageData = File.ReadAllBytes(Path.Combine(Constants.sourcePath, "example.png"));
        var worksheet = workbook.Worksheets[0];
        var chart = worksheet.Charts[0];
        chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
        chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
        chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
        chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
        chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;

        workbook.Save(Constants.destPath + "example.xls");
    }
    using (Workbook workbook = new Workbook(Constants.destPath + "example.xls"))
    {
        Chart chart = workbook.Worksheets[0].Charts[0];
        Assert.AreEqual(chart.ChartArea.Area.FillFormat.FillType, FillType.Texture);
        Util.SaveManCheck(workbook, "Shape", "example.xls");
    }

}
```

### See Also

* class [TilePicOption](../../tilepicoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


