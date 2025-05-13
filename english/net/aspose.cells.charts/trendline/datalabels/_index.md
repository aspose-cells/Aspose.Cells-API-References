---
title: Trendline.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Represents the DataLabels object for the specified series
type: docs
url: /net/aspose.cells.charts/trendline/datalabels/
---
## Trendline.DataLabels property

Represents the DataLabels object for the specified series.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
// Called: chart.NSeries[1].TrendLines[0].DataLabels.Y = -694;
public void Trendline_Property_DataLabels(Workbook workbook)
        {
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet sheet = workbook.Worksheets[sheetIndex];
            //Set the name of worksheet
            sheet.Name = "Chart";

            //Create chart
            int chartIndex = 0;
            chartIndex = sheet.Charts.Add(ChartType.ScatterConnectedByLinesWithDataMarker, 1, 1, 25, 10);
            Chart chart = sheet.Charts[chartIndex];

            //Set properties of chart
            chart.CategoryAxis.MajorGridLines.IsVisible = false;
            chart.Legend.Position = LegendPositionType.Top;

            //Set properties of chart title
            chart.Title.Text = "Scatter Chart:Particulate Levels in Rainfall";
            chart.Title.Font.Color = Color.Black;
            chart.Title.Font.IsBold = true;
            chart.Title.Font.Size = 12;

            //Set properties of nseries
            chart.NSeries.Add("Data!B2:B10", true);
            chart.NSeries[0].XValues = "Data!A2:A10";

            for (int i = 0; i <= chart.NSeries.Count - 1; i++)
            {
                chart.NSeries[i].Name = "Particulate";
            }

            //Trend Lines
            chart.NSeries.Add("Data!B2:B10", true);
            chart.NSeries[1].XValues = "Data!A2:A10";
            chart.NSeries[1].Type = ChartType.Scatter;
            chart.NSeries[1].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic");
            chart.NSeries[1].TrendLines[0].Order = 2;
            chart.NSeries[1].TrendLines[0].Style = Aspose.Cells.Drawing.LineType.Solid;
            chart.NSeries[1].TrendLines[0].DisplayRSquared = true;
            chart.NSeries[1].TrendLines[0].DataLabels.Border.IsVisible = true;
            chart.NSeries[1].TrendLines[0].DataLabels.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
            chart.NSeries[1].TrendLines[0].DataLabels.Border.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
            chart.NSeries[1].TrendLines[0].DataLabels.Border.Color = Color.Black;
            chart.NSeries[1].TrendLines[0].DataLabels.Font.Color = Color.Blue;
            //chart.NSeries[1].DataLabels.ShowCategoryName = true;
            //chart.NSeries[1].DataLabels.ShowSeriesName = true;
            //chart.NSeries[1].DataLabels.ShowValue = true;
            //chart.NSeries[1].DataLabels.Position = LabelPositionType.Left;
            chart.NSeries[1].TrendLines[0].DataLabels.X = -1608;
            chart.NSeries[1].TrendLines[0].DataLabels.Y = -694;

            Cells cells = workbook.Worksheets[0].Cells;
            //Set properties of categoryaxis title
            chart.CategoryAxis.Title.Text = cells["A1"].Value.ToString();
            chart.CategoryAxis.Title.Font.Color = Color.Black;
            chart.CategoryAxis.Title.Font.IsBold = true;
            chart.CategoryAxis.Title.Font.Size = 10;

            //Set properties of valueaxis title
            chart.ValueAxis.Title.Text = cells["B1"].Value.ToString();
            chart.ValueAxis.Title.Font.Color = Color.Black;
            chart.ValueAxis.Title.Font.IsBold = true;
            chart.ValueAxis.Title.Font.Size = 10;
            chart.ValueAxis.Title.RotationAngle = 90;
        }
```

### See Also

* class [DataLabels](../../datalabels/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


