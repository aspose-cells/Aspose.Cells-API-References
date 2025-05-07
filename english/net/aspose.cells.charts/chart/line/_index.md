---
title: Chart.Line
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the line
type: docs
url: /net/aspose.cells.charts/chart/line/
---
## Chart.Line property

Gets the line.

```csharp
public Line Line { get; }
```

### Examples

```csharp
// Called: Line line = chart.Line;
public static void Property_Line()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
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

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Create a line shape for the chart
            Line line = chart.Line;

            // Set arrowhead styles and widths
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // Output the arrowhead styles and widths
            Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowWidth);
            Console.WriteLine("End Arrowhead Width: " + line.EndArrowWidth);

            // Save the workbook
            workbook.Save("MsoArrowheadWidthExample.xlsx");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


