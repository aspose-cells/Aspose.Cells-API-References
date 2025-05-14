---
title: Trendline.Intercept
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Returns or sets the point where the trendline crosses the value axis
type: docs
url: /net/aspose.cells.charts/trendline/intercept/
---
## Trendline.Intercept property

Returns or sets the point where the trendline crosses the value axis.

```csharp
public double Intercept { get; set; }
```

### Examples

```csharp
// Called: trendline.Intercept = 0.0;
public static void Trendline_Property_Intercept()
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
            chart.NSeries.Add("A1:B4", true);
            // Setting the data source for the category data of NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Adding a linear trendline
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            // Setting the custom name of the trendline
            trendline.Name = "Linear";
            // Displaying the equation on chart
            trendline.DisplayEquation = true;
            // Displaying the R-Squared value on chart
            trendline.DisplayRSquared = true;

            // Setting additional properties
            trendline.IsNameAuto = false;
            trendline.Order = 2;
            trendline.Period = 3;
            trendline.Forward = 1.5;
            trendline.Backward = 0.5;
            trendline.Intercept = 0.0;
            trendline.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
            trendline.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.Dash;
            trendline.CapType = Aspose.Cells.Drawing.LineCapType.Round;
            trendline.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
            trendline.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
            trendline.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
            trendline.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
            trendline.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
            trendline.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
            trendline.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
            trendline.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
            trendline.Color = Color.Red;
            trendline.Transparency = 0.5;
            trendline.Style = Aspose.Cells.Drawing.LineType.DashDot;
            trendline.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
            trendline.WeightPt = 2.0;
            trendline.WeightPx = 3.0;
            trendline.FormattingType = Aspose.Cells.Charts.ChartLineFormattingType.Gradient;
            trendline.IsVisible = true;
            trendline.IsAuto = false;

            // Saving the Excel file
            workbook.Save("TrendlineExample.xlsx");
        }
```

### See Also

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


