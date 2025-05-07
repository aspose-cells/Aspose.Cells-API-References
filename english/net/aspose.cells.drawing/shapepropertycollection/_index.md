---
title: Class ShapePropertyCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShapePropertyCollection class. This class specifies the visual shape properties for a chart element or shape
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/
---
## ShapePropertyCollection class

This class specifies the visual shape properties for a chart element or shape.

```csharp
public class ShapePropertyCollection
```

## Properties

| Name | Description |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | Represents a [`Format3D`](./format3d/) object that specifies 3D shape properties for the chart element or shape. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | Represents a [`GlowEffect`](./gloweffect/) object that specifies glow effect for the chart element or shape. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | Represents a [`ShadowEffect`](./shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | Gets and sets the radius of blur to apply to the edges, in unit of points. |

## Methods

| Name | Description |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | Clears the 3D shape properties of the shape. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | Clears the glow effect of the shape. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | Clears the shadow effect of the chart element or shape. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | Indicates if the shape has 3d format data. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | Indicates if the shape has glow effect data. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | Indicates if the shape has shadow effect data. |

### Examples

```csharp
// Called: ShapePropertyCollection spPr = ser.ShapeProperties;
[Test]
        //http://www.aspose.com/community/forums/thread/262927.aspx
        public void Type_ShapePropertyCollection()
        {
            Console.WriteLine("Type_ShapePropertyCollection()");
            string outfn = Constants.destPath + "chart_out.xlsx";

            Workbook book = new Workbook();
            Worksheet dataSheet = book.Worksheets.Add("DataSheet");
            Worksheet sheet = book.Worksheets.Add("MyChart");

            dataSheet.Cells["B1"].PutValue(1);
            dataSheet.Cells["B2"].PutValue(2);
            dataSheet.Cells["B3"].PutValue(3);
            dataSheet.Cells["A1"].PutValue("A");
            dataSheet.Cells["A2"].PutValue("B");
            dataSheet.Cells["A3"].PutValue("C");

            ChartCollection charts = sheet.Charts;
            int chartSheetIdx = charts.Add(ChartType.Column, 5, 0, 25, 15);
            Aspose.Cells.Charts.Chart chart = book.Worksheets[2].Charts[0];
            chart.PlotArea.Area.BackgroundColor = Color.White;
            chart.ChartArea.Area.BackgroundColor = Color.White;
            chart.PlotArea.Area.ForegroundColor = Color.White;
            chart.ChartArea.Area.ForegroundColor = Color.White;
            chart.ValueAxis.MajorGridLines.Color = Color.Silver;
            chart.ValueAxis.AxisLine.Color = Color.Silver;
            chart.CategoryAxis.AxisLine.Color = Color.Silver;

            chart.ShowLegend = false;
            chart.NSeries.Add("DataSheet!B1:B3", true);
            chart.NSeries.CategoryData = "DataSheet!A1:A3";

            Aspose.Cells.Charts.Series ser = chart.NSeries[0];

            ShapePropertyCollection spPr = ser.ShapeProperties;
            Format3D fmt3d = spPr.Format3D;
            Bevel bevel = fmt3d.TopBevel;

            bevel.Type = BevelPresetType.Circle;
            bevel.Height = 2;
            bevel.Width = 5;

            //bevel.Type = BevelPresetType.RelaxedInset;
            //bevel.Height = 10;
            //bevel.Width = 10;

            fmt3d.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            fmt3d.SurfaceLightingType = LightRigType.ThreePoint;
            fmt3d.LightingAngle = 20;
            //fmt3d.SurfaceLightingType = LightRigType.Balanced;
            //fmt3d.LightingAngle = 70;

            //for (int x = 0; x < chart.NSeries[0].Points.Count; x++)
            //{
            //  chart.NSeries[0].Points[x].Area.BackgroundColor = Color.Blue;
            //  chart.NSeries[0].Points[x].Area.ForegroundColor = Color.Blue;
            //  chart.NSeries[0].Points[x].Border.Color = Color.Blue;
            //}
            ser.Area.BackgroundColor = Color.Blue;
            ser.Area.ForegroundColor = Color.Blue;
            ser.Border.Color = Color.Blue;

            //book.Worksheets.SetOleSize(0, 3, 0, 1);
            book.Save(outfn, SaveFormat.Xlsx);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


