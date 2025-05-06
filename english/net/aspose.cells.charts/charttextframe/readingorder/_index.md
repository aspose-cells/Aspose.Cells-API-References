---
title: ChartTextFrame.ReadingOrder
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Represents text reading order
type: docs
url: /net/aspose.cells.charts/charttextframe/readingorder/
---
## ChartTextFrame.ReadingOrder property

Represents text reading order.

```csharp
public TextDirectionType ReadingOrder { get; set; }
```

### Examples

```csharp
// Called: chart.Title.ReadingOrder = TextDirectionType.LeftToRight;
public static void Property_ReadingOrder()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Access the first worksheet
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue(&quot;Income&quot;);
            cells[1, 0].PutValue(&quot;Company A&quot;);
            cells[2, 0].PutValue(&quot;Company B&quot;);
            cells[3, 0].PutValue(&quot;Company C&quot;);
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Add a chart to the worksheet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];

            // Set the data source for the chart
            chart.NSeries.Add(&quot;B2:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;A2:A4&quot;;

            // Set the title of the chart
            chart.Title.Text = &quot;Income Analysis&quot;;
            chart.Title.Font.Color = Color.Blue;
            chart.Title.IsVisible = true;
            chart.Title.X = 100;
            chart.Title.Y = 50;
            chart.Title.OverLay = false;
            chart.Title.IsAutoText = false;
            chart.Title.IsDeleted = false;
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Center;
            chart.Title.RotationAngle = 0;
            chart.Title.LinkedSource = null;
            chart.Title.TextDirection = TextDirectionType.LeftToRight;
            chart.Title.ReadingOrder = TextDirectionType.LeftToRight;
            chart.Title.DirectionType = ChartTextDirectionType.Horizontal;
            chart.Title.IsTextWrapped = true;
            chart.Title.IsResizeShapeToFitText = true;
            chart.Title.IsInnerMode = false;
            chart.Title.AutoScaleFont = true;
            chart.Title.BackgroundMode = BackgroundMode.Transparent;
            chart.Title.IsAutomaticSize = true;
            chart.Title.Height = 100;
            chart.Title.Width = 200;
            chart.Title.Shadow = false;

            // Save the workbook
            workbook.Save(&quot;TitleExample.xlsx&quot;);
        }
```

### See Also

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


