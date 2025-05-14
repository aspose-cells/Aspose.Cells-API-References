---
title: Marker.MarkerSize
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker size in unit of points. Applies to line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart.

```csharp
public int MarkerSize { get; set; }
```

### Examples

```csharp
// Called: aSerie.Marker.MarkerSize = 3;
public void Marker_Property_MarkerSize()
        {
            Console.WriteLine("Marker_Property_MarkerSize()");
            Workbook wb = new Workbook();
            wb.Worksheets.Clear();

            Worksheet ws = wb.Worksheets.Add("New");
            Style style = wb.CreateStyle();
            style.Name = "DateTimeStyle";
            style.Custom = "dd-mm hh:mm:ss";
            DateTime dt = DateTime.Now.Date;
            ws.Cells[23, 2].PutValue(dt);
            ws.Cells[23, 2].SetStyle(style);
            ws.Cells[24, 2].PutValue(dt.AddHours(1));
            ws.Cells[24, 2].SetStyle(style);
            ws.Cells[25, 2].PutValue(dt.AddHours(2));
            ws.Cells[25, 2].SetStyle(style);
            ws.Cells[26, 2].PutValue(dt.AddHours(3));
            ws.Cells[26, 2].SetStyle(style);
            ws.Cells[27, 2].PutValue(dt.AddHours(4));
            ws.Cells[27, 2].SetStyle(style);
            ws.Cells[28, 2].PutValue(dt.AddHours(5));
            ws.Cells[28, 2].SetStyle(style);
            ws.Cells[29, 2].PutValue(dt.AddHours(6));
            ws.Cells[29, 2].SetStyle(style);
            ws.Cells[23, 3].PutValue(3);
            ws.Cells[24, 3].PutValue(4);
            ws.Cells[25, 3].PutValue(9);
            ws.Cells[26, 3].PutValue(13);
            ws.Cells[27, 3].PutValue(16);
            ws.Cells[28, 3].PutValue(3);
            ws.Cells[29, 3].PutValue(7);

            Chart chart = ws.Charts[ws.Charts.Add(ChartType.ScatterConnectedByLinesWithoutDataMarker, 1, 1, 22, 12)];
            chart.CategoryAxis.TickLabels.NumberFormat = "dd-mm hh:mm;@";
            chart.CategoryAxis.TickLabels.RotationAngle = 45;
            chart.CategoryAxis.TickLabels.Font.Size = 8;
            chart.CategoryAxis.MinValue = dt;
            chart.CategoryAxis.MaxValue = dt.AddHours(6);
            double d = 1f / 24f;
            chart.CategoryAxis.MajorUnit = 0.04166666;
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.ValueAxis.TickLabels.NumberFormat = "0";
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 20;
            chart.Placement = PlacementType.Move;
            String chartSubTitle = DateTime.Now.ToString();
            chart.Title.Text = "Data" + "\n" + chartSubTitle;
            FontSetting chars = chart.Title.Characters(chart.Title.Text.Length - chartSubTitle.Length, chartSubTitle.Length);
            chars.Font.Size = 10;
            chars.Font.IsBold = false;
            chart.ValueAxis.Title.Text = "unit";

            Series aSerie = chart.NSeries[chart.NSeries.Add(String.Format("{0}!{1}{2}:{1}{3}", ws.Name, "D", 24, 30), true)];
            aSerie.XValues = String.Format("{0}!{1}{2}:{1}{3}", ws.Name, "C", 24, 30);
            aSerie.Name = "Date";
            aSerie.Border.Color = Color.YellowGreen;
            aSerie.Border.Weight = WeightType.HairLine;
            aSerie.Marker.MarkerStyle = ChartMarkerType.Diamond;
            aSerie.Marker.BackgroundColorSetType = FormattingType.Automatic;
            aSerie.Marker.BackgroundColor = Color.YellowGreen;
            aSerie.Marker.ForegroundColorSetType = FormattingType.None;
            aSerie.Marker.MarkerSize = 3;

            wb.Save(path + "Result.xlsx");
        }
```

### See Also

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


