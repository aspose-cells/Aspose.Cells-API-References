---
title: ChartFrame.Background
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets and sets the display mode of the background
type: docs
url: /net/aspose.cells.charts/chartframe/background/
---
## ChartFrame.Background property

Gets and sets the display mode of the background

```csharp
[Obsolete("Use ChartFrame.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: dataLabels.Background = BackgroundMode.Transparent;
public static void Property_Background()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add(&quot;B2:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;A2:A4&quot;;

            // Access the DataLabels of the first series
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Set properties of DataLabels
            dataLabels.Position = LabelPositionType.InsideBase;
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.ShowPercentage = false;
            dataLabels.ShowLegendKey = false;
            dataLabels.IsAutoText = true;
            dataLabels.DirectionType = ChartTextDirectionType.Horizontal;
            dataLabels.Text = &quot;Custom Text&quot;;
            dataLabels.IsTextWrapped = true;
            dataLabels.BackgroundMode = BackgroundMode.Transparent;
            dataLabels.ShowCellRange = false;
            dataLabels.ShowBubbleSize = false;
            dataLabels.ShowSeriesName = false;
            dataLabels.NumberFormat = &quot;0.00&quot;;
            dataLabels.Number = 0;
            dataLabels.NumberFormatLinked = false;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
            dataLabels.SeparatorValue = &quot;, &quot;;
            dataLabels.IsNeverOverlap = true;
            dataLabels.IsDeleted = false;
            dataLabels.TextHorizontalAlignment = TextAlignmentType.Center;
            dataLabels.TextVerticalAlignment = TextAlignmentType.Center;
            dataLabels.RotationAngle = 0;
            dataLabels.LinkedSource = &quot;&quot;;
            dataLabels.TextDirection = TextDirectionType.LeftToRight;
            dataLabels.ReadingOrder = TextDirectionType.LeftToRight;
            dataLabels.IsResizeShapeToFitText = true;
            dataLabels.IsInnerMode = false;
            dataLabels.AutoScaleFont = true;
            dataLabels.Background = BackgroundMode.Transparent;
            dataLabels.IsAutomaticSize = true;
            dataLabels.X = 0;
            dataLabels.Y = 0;
            dataLabels.Height = 100;
            dataLabels.Width = 100;
            dataLabels.Shadow = false;

            // Save the workbook
            workbook.Save(&quot;DataLabelsExample.xlsx&quot;);
            workbook.Save(&quot;DataLabelsExample.pdf&quot;);
        }
```

### See Also

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


