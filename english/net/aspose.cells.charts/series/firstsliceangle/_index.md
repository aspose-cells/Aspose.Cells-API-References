---
title: Series.FirstSliceAngle
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets or sets the angle of the first piechart or doughnutchart slice in degrees clockwise from vertical. Applies only to pie 3D pie and doughnut charts 0 to 360
type: docs
url: /net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

```csharp
public short FirstSliceAngle { get; set; }
```

### Examples

```csharp
// Called: series.FirstSliceAngle = 45;
public static void Property_FirstSliceAngle()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Adding a new worksheet to the Excel object
            int sheetIndex = workbook.Worksheets.Add();
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Adding sample values to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;A4&quot;].PutValue(200);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            worksheet.Cells[&quot;B4&quot;].PutValue(40);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Q1&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(&quot;Q2&quot;);
            worksheet.Cells[&quot;C3&quot;].PutValue(&quot;Y1&quot;);
            worksheet.Cells[&quot;C4&quot;].PutValue(&quot;Y2&quot;);

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];
            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B4&quot;
            int seriesIndex = chart.NSeries.Add(&quot;A1:B4&quot;, true);
            // Setting the data source for the category data of NSeries
            chart.NSeries.CategoryData = &quot;C1:C4&quot;;

            // Accessing the series
            Series series = chart.NSeries[seriesIndex];

            // Setting the values of the series
            series.Values = &quot;=B1:B4&quot;;
            // Changing the chart type of the series
            series.Type = ChartType.Line;
            // Setting marker properties
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Setting additional properties
            series.Name = &quot;First Series&quot;;
            series.IsFiltered = false;
            series.ValuesFormatCode = &quot;0.00&quot;;
            series.XValues = &quot;=A1:A4&quot;;
            series.BubbleSizes = &quot;=B1:B4&quot;;
            series.Smooth = true;
            series.Shadow = true;
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;
            series.PlotOnSecondAxis = false;
            series.HasHiLoLines = false;
            series.HasSeriesLines = false;
            series.HasDropLines = false;
            series.HasUpDownBars = false;
            series.IsColorVaried = false;
            series.GapWidth = 150;
            series.FirstSliceAngle = 45;
            series.Overlap = 0;
            series.SecondPlotSize = 100;
            series.SplitType = ChartSplitType.Position;
            series.SplitValue = 10.0;
            series.BubbleScale = 100;
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;
            series.ShowNegativeBubbles = true;
            series.DoughnutHoleSize = 50;
            series.Explosion = 10;
            series.HasRadarAxisLabels = false;
            series.HasLeaderLines = true;

            // Saving the Excel file
            workbook.Save(&quot;SeriesExample.xlsx&quot;);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


