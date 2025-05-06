---
title: TickLabels.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Represents the format string for the TickLabels object
type: docs
url: /net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

Represents the format string for the TickLabels object.

```csharp
public string NumberFormat { get; set; }
```

### Remarks

The formatting string is same as a custom format string setting to a cell. For example, "$0".

### Examples

```csharp
// Called: chart.ValueAxis.TickLabels.NumberFormat = &amp;quot;0&amp;quot;;
[Test]
        //http://www.aspose.com/community/forums/thread/255754.aspx
        public void Property_NumberFormat()
        {
            Console.WriteLine(&quot;Property_NumberFormat()&quot;);
            string outfn = Constants.destPath + &quot;Test_SerLineStyle_out.xlsx&quot;;

            Workbook wb = new Workbook();

            wb.Worksheets.Clear();

            Worksheet ws = wb.Worksheets.Add(&quot;New&quot;);

            Style style = wb.CreateStyle();

            style.Name = &quot;DateTimeStyle&quot;;

            style.Custom = &quot;dd-mm hh:mm:ss&quot;;

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

            chart.CategoryAxis.TickLabels.NumberFormat = &quot;dd-mm hh:mm;@&quot;;

            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            chart.CategoryAxis.TickLabels.Font.Size = 8;

            chart.CategoryAxis.MinValue = dt;

            chart.CategoryAxis.MaxValue = dt.AddHours(6);

            double d = 1f / 24f;

            chart.CategoryAxis.MajorUnit = 0.04166666;

            chart.Legend.Position = LegendPositionType.Bottom;

            chart.ValueAxis.TickLabels.NumberFormat = &quot;0&quot;;

            chart.ValueAxis.MinValue = 0;

            chart.ValueAxis.MaxValue = 20;

            chart.Placement = PlacementType.Move;

            String chartSubTitle = DateTime.Now.ToString();

            chart.Title.Text = &quot;Data&quot; + &quot;\n&quot; + chartSubTitle;

            FontSetting chars = chart.Title.Characters(chart.Title.Text.Length - chartSubTitle.Length, chartSubTitle.Length);

            chars.Font.Size = 10;

            chars.Font.IsBold = false;

            chart.ValueAxis.Title.Text = &quot;unit&quot;;

            Series aSerie = chart.NSeries[chart.NSeries.Add(String.Format(&quot;{0}!{1}{2}:{1}{3}&quot;, ws.Name, &quot;D&quot;, 24, 30), true)];

            aSerie.XValues = String.Format(&quot;{0}!{1}{2}:{1}{3}&quot;, ws.Name, &quot;C&quot;, 24, 30);

            aSerie.Name = &quot;Date&quot;;

            aSerie.Border.Color = Color.YellowGreen;

            aSerie.Border.Weight = WeightType.HairLine;

            aSerie.Marker.MarkerStyle = ChartMarkerType.Diamond;

            aSerie.Marker.Area.Formatting = FormattingType.Automatic;

            aSerie.Marker.Area.ForegroundColor = Color.YellowGreen;

            aSerie.Marker.Border.FormattingType = ChartLineFormattingType.None;

            aSerie.Marker.MarkerSize = 3;

            wb.Save(outfn);
        }
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


