---
title: ChartTextFrame.Text
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets or sets the text of a frames title
type: docs
url: /net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

Gets or sets the text of a frame's title.

```csharp
public virtual string Text { get; set; }
```

### Examples

```csharp
// Called: title.Text = &amp;quot;Sample Chart&amp;quot;;
public static void Property_Text()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
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

            // Access the chart title
            ChartTextFrame title = chart.Title;
            title.Text = &quot;Sample Chart&quot;;
            title.TextHorizontalAlignment = TextAlignmentType.Center;
            title.TextVerticalAlignment = TextAlignmentType.Center;
            title.RotationAngle = 0;
            title.IsAutoText = false;
            title.IsDeleted = false;
            title.TextDirection = TextDirectionType.LeftToRight;
            title.ReadingOrder = TextDirectionType.LeftToRight;
            title.DirectionType = ChartTextDirectionType.Horizontal;
            title.IsTextWrapped = true;
            title.IsResizeShapeToFitText = true;
            title.IsInnerMode = false;
            title.AutoScaleFont = true;
            title.BackgroundMode = BackgroundMode.Transparent;
            title.IsAutomaticSize = true;
            title.X = 0;
            title.Y = 0;
            title.Height = 400;
            title.Width = 400;
            title.Shadow = true;

            // Save the workbook
            workbook.Save(&quot;ChartTextFrameExample.xlsx&quot;);
            workbook.Save(&quot;ChartTextFrameExample.pdf&quot;);
        }
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


