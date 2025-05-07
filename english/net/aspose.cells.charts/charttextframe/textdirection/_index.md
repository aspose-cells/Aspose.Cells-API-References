---
title: ChartTextFrame.TextDirection
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Represents text reading order
type: docs
url: /net/aspose.cells.charts/charttextframe/textdirection/
---
## ChartTextFrame.TextDirection property

Represents text reading order.

```csharp
[Obsolete("Use ChartTextFrame.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: title.TextDirection = TextDirectionType.LeftToRight;
public static void Property_TextDirection()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Access the chart title
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
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
            workbook.Save("ChartTextFrameExample.xlsx");
            workbook.Save("ChartTextFrameExample.pdf");
        }
```

### See Also

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


