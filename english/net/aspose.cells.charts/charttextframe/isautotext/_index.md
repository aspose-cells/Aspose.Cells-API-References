---
title: ChartTextFrame.IsAutoText
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Indicates the text is auto generated
type: docs
url: /net/aspose.cells.charts/charttextframe/isautotext/
---
## ChartTextFrame.IsAutoText property

Indicates the text is auto generated.

```csharp
public virtual bool IsAutoText { get; set; }
```

### Examples

```csharp
// Called: title.IsAutoText = false;
public static void ChartTextFrame_Property_IsAutoText()
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

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


