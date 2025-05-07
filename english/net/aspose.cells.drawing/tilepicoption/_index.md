---
title: Class TilePicOption
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.TilePicOption class. Represents tile picture as texture
type: docs
url: /net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

Represents tile picture as texture.

```csharp
public class TilePicOption
```

## Constructors

| Name | Description |
| --- | --- |
| [TilePicOption](tilepicoption/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Gets or sets the alignment for tiling. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Gets or sets the mirror type for tiling. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Gets or sets the X offset for tiling picture. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Gets or sets the Y offset for tiling picture. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Gets or sets the X scale for tiling picture. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Gets or sets the Y scale for tiling picture. |

### Examples

```csharp
// Called: chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
[Test]
        public void Type_TilePicOption()
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

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


