---
title: Series.Has3DEffect
second_title: Aspose.Cells for .NET API Reference
description: Series property. True if the series has a threedimensional appearance. Applies only to bubble charts
type: docs
url: /net/aspose.cells.charts/series/has3deffect/
---
## Series.Has3DEffect property

True if the series has a three-dimensional appearance. Applies only to bubble charts.

```csharp
public bool Has3DEffect { get; set; }
```

### Examples

```csharp
// Called: series.Has3DEffect = true;
public static void Series_Property_Has3DEffect()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Adding a new worksheet to the Excel object
            int sheetIndex = workbook.Worksheets.Add();
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Adding sample values to cells
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];
            // Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Setting the data source for the category data of NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Accessing the series
            Series series = chart.NSeries[seriesIndex];

            // Setting the values of the series
            series.Values = "=B1:B4";
            // Changing the chart type of the series
            series.Type = ChartType.Line;
            // Setting marker properties
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Setting additional properties
            series.Name = "First Series";
            series.IsFiltered = false;
            series.ValuesFormatCode = "0.00";
            series.XValues = "=A1:A4";
            series.BubbleSizes = "=B1:B4";
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
            workbook.Save("SeriesExample.xlsx");
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


