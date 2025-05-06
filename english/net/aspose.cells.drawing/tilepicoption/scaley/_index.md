---
title: TilePicOption.ScaleY
second_title: Aspose.Cells for .NET API Reference
description: TilePicOption property. Gets or sets the Y scale for tiling picture
type: docs
url: /net/aspose.cells.drawing/tilepicoption/scaley/
---
## TilePicOption.ScaleY property

Gets or sets the Y scale for tiling picture.

```csharp
public double ScaleY { get; set; }
```

### Examples

```csharp
// Called: chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
[Test]
        public void Property_ScaleY()
        {
            using (Workbook workbook = new Workbook(Path.Combine(Constants.sourcePath, &quot;CellsNet45362.xls&quot;)))
            {
                var imageData = File.ReadAllBytes(Path.Combine(Constants.sourcePath, &quot;CellsNet45361.png&quot;));
                var worksheet = workbook.Worksheets[0];
                var chart = worksheet.Charts[0];
                chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
                chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
                chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
                chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
                chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;

                workbook.Save(Constants.destPath + &quot;CellsNet45362.xls&quot;);
            }
            using (Workbook workbook = new Workbook(Constants.destPath + &quot;CellsNet45362.xls&quot;))
            {
                Chart chart = workbook.Worksheets[0].Charts[0];
                Assert.AreEqual(chart.ChartArea.Area.FillFormat.FillType, FillType.Texture);
                Util.SaveManCheck(workbook, &quot;Shape&quot;, &quot;CellsNet45362.xls&quot;);
            }

        }
```

### See Also

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


