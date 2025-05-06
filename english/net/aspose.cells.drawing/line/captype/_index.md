---
title: Line.CapType
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the ending caps
type: docs
url: /net/aspose.cells.drawing/line/captype/
---
## Line.CapType property

Specifies the ending caps.

```csharp
public LineCapType CapType { get; set; }
```

### Examples

```csharp
// Called: trendline.CapType = Aspose.Cells.Drawing.LineCapType.Round;
public static void Property_CapType()
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
            chart.NSeries.Add(&quot;A1:B4&quot;, true);
            // Setting the data source for the category data of NSeries
            chart.NSeries.CategoryData = &quot;C1:C4&quot;;

            // Adding a linear trendline
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            // Setting the custom name of the trendline
            trendline.Name = &quot;Linear&quot;;
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
            workbook.Save(&quot;TrendlineExample.xlsx&quot;);
        }
```

### See Also

* enum [LineCapType](../../linecaptype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


