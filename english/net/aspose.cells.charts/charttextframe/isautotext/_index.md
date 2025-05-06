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
// Called: displayUnitLabel.IsAutoText = false;
public static void Property_IsAutoText()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            // Adding a new worksheet to the Workbook object
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

            // Setting the display unit of value(Y) axis
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Setting properties of DisplayUnitLabel
            displayUnitLabel.Text = &quot;100&quot;;
            displayUnitLabel.AutoScaleFont = true;
            displayUnitLabel.IsAutoText = false;
            displayUnitLabel.IsDeleted = false;
            displayUnitLabel.TextHorizontalAlignment = TextAlignmentType.Center;
            displayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;
            displayUnitLabel.RotationAngle = 0;
            displayUnitLabel.LinkedSource = &quot;&quot;;
            displayUnitLabel.TextDirection = TextDirectionType.LeftToRight;
            displayUnitLabel.ReadingOrder = TextDirectionType.LeftToRight;
            displayUnitLabel.DirectionType = ChartTextDirectionType.Horizontal;
            displayUnitLabel.IsTextWrapped = false;
            displayUnitLabel.IsResizeShapeToFitText = false;
            displayUnitLabel.IsInnerMode = false;
            displayUnitLabel.BackgroundMode = BackgroundMode.Transparent;
            displayUnitLabel.IsAutomaticSize = true;
            displayUnitLabel.X = 0;
            displayUnitLabel.Y = 0;
            displayUnitLabel.Height = 100;
            displayUnitLabel.Width = 100;
            displayUnitLabel.Shadow = false;

            // Saving the Excel file
            workbook.Save(&quot;DisplayUnitLabelExample.xlsx&quot;);
            workbook.Save(&quot;DisplayUnitLabelExample.pdf&quot;);
        }
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


