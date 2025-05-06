---
title: Series.YErrorBar
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents Y direction error bar of the series
type: docs
url: /net/aspose.cells.charts/series/yerrorbar/
---
## Series.YErrorBar property

Represents Y direction error bar of the series.

```csharp
public ErrorBar YErrorBar { get; }
```

### Examples

```csharp
// Called: series.YErrorBar.IsVisible = true;
public static void Property_YErrorBar()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Add sample data to cells
            cells[&quot;A1&quot;].PutValue(2);
            cells[&quot;A2&quot;].PutValue(5);
            cells[&quot;A3&quot;].PutValue(3);
            cells[&quot;A4&quot;].PutValue(6);
            cells[&quot;B1&quot;].PutValue(4);
            cells[&quot;B2&quot;].PutValue(3);
            cells[&quot;B3&quot;].PutValue(6);
            cells[&quot;B4&quot;].PutValue(7);
            cells[&quot;C1&quot;].PutValue(&quot;Q1&quot;);
            cells[&quot;C2&quot;].PutValue(&quot;Q2&quot;);
            cells[&quot;C3&quot;].PutValue(&quot;Y1&quot;);
            cells[&quot;C4&quot;].PutValue(&quot;Y2&quot;);

            // Add a chart to the worksheet
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];

            // Add NSeries (chart data source) to the chart
            chart.NSeries.Add(&quot;A1:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;C1:C4&quot;;

            // Configure error bars for each series in the chart
            for (int i = 0; i &lt; chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;

                // Additional properties for demonstration
                series.YErrorBar.ShowMarkerTTop = true;
                series.YErrorBar.PlusValue = &quot;=Sheet1!A1&quot;;
                series.YErrorBar.MinusValue = &quot;=Sheet1!A2&quot;;
                series.YErrorBar.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
                series.YErrorBar.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.DashDot;
                series.YErrorBar.CapType = Aspose.Cells.Drawing.LineCapType.Round;
                series.YErrorBar.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
                series.YErrorBar.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
                series.YErrorBar.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.ArrowDiamond;
                series.YErrorBar.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
                series.YErrorBar.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
                series.YErrorBar.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
                series.YErrorBar.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
                series.YErrorBar.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
                series.YErrorBar.Color = System.Drawing.Color.Red;
                series.YErrorBar.Transparency = 0.5;
                series.YErrorBar.Style = Aspose.Cells.Drawing.LineType.DashDotDot;
                series.YErrorBar.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
                series.YErrorBar.WeightPt = 2.0;
                series.YErrorBar.WeightPx = 3.0;
                series.YErrorBar.FormattingType = ChartLineFormattingType.Gradient;
                series.YErrorBar.IsVisible = true;
                series.YErrorBar.IsAuto = false;
            }

            // Save the workbook
            workbook.Save(&quot;ErrorBarExample.xlsx&quot;);
            workbook.Save(&quot;ErrorBarExample.pdf&quot;);
        }
```

### See Also

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


