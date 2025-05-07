---
title: TilePicOption.ScaleX
second_title: Aspose.Cells for .NET API Reference
description: TilePicOption property. Gets or sets the X scale for tiling picture
type: docs
url: /net/aspose.cells.drawing/tilepicoption/scalex/
---
## TilePicOption.ScaleX property

Gets or sets the X scale for tiling picture.

```csharp
public double ScaleX { get; set; }
```

### Examples

```csharp
// Called: chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
[Test]
        public void Property_ScaleX()
        {
            using (Workbook workbook = new Workbook(Path.Combine(Constants.sourcePath, "CellsNet45362.xls")))
            {
                var imageData = File.ReadAllBytes(Path.Combine(Constants.sourcePath, "CellsNet45361.png"));
                var worksheet = workbook.Worksheets[0];
                var chart = worksheet.Charts[0];
                chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
                chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
                chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
                chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
                chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;

                workbook.Save(Constants.destPath + "CellsNet45362.xls");
            }
            using (Workbook workbook = new Workbook(Constants.destPath + "CellsNet45362.xls"))
            {
                Chart chart = workbook.Worksheets[0].Charts[0];
                Assert.AreEqual(chart.ChartArea.Area.FillFormat.FillType, FillType.Texture);
                Util.SaveManCheck(workbook, "Shape", "CellsNet45362.xls");
            }

        }
```

### See Also

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


