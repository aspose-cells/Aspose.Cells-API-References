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
[Test]
        public void Property_TilePicOption()
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

* class [TilePicOption](../../tilepicoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


