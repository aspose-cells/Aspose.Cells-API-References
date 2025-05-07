---
title: Bevel.Width
second_title: Aspose.Cells for .NET API Reference
description: Bevel property. Gets and sets the width of the bevel or how far into the shape it is applied. In unit of Points
type: docs
url: /net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points.

```csharp
public double Width { get; set; }
```

### Examples

```csharp
// Called: bevel.Width = 5;
[Test]
        //http://www.aspose.com/community/forums/thread/262927.aspx
        public void Property_Width()
        {
            Console.WriteLine("Property_Width()");
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

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


