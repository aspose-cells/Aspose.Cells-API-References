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
// Called: legend.Text = "Legend Text";
public static void ChartTextFrame_Property_Text()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Get the first worksheet
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Add a chart to the worksheet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Access the legend of the chart
            Legend legend = chart.Legend;

            // Set legend properties
            legend.Position = LegendPositionType.Left;
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;
            legend.IsOverLay = false;
            legend.IsAutoText = true;
            legend.IsDeleted = false;
            legend.TextHorizontalAlignment = TextAlignmentType.Center;
            legend.TextVerticalAlignment = TextAlignmentType.Center;
            legend.RotationAngle = 0;
            legend.Text = "Legend Text";
            legend.LinkedSource = "Sheet1!A1";
            legend.TextDirection = TextDirectionType.LeftToRight;
            legend.ReadingOrder = TextDirectionType.Context;
            legend.DirectionType = ChartTextDirectionType.Horizontal;
            legend.IsTextWrapped = true;
            legend.IsResizeShapeToFitText = true;
            legend.IsInnerMode = false;
            legend.AutoScaleFont = true;
            legend.BackgroundMode = BackgroundMode.Transparent;
            legend.IsAutomaticSize = true;
            legend.X = 100;
            legend.Y = 100;
            legend.Height = 200;
            legend.Width = 200;
            legend.Shadow = true;

            // Save the workbook
            workbook.Save("LegendExample.xlsx");
            workbook.Save("LegendExample.pdf");
        }
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


