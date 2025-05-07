---
title: Enum MsoArrowheadStyle
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.MsoArrowheadStyle enum. Enumerates the line end type of the shape border line
type: docs
url: /net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Enumerates the line end type of the shape border line.

```csharp
public enum MsoArrowheadStyle
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No line end type. |
| Arrow | `1` | Arrow line end type. |
| ArrowStealth | `2` | Arrow Stealth line end type. |
| ArrowDiamond | `3` | Arrow Diamond Line end type. |
| ArrowOval | `4` | Arrow Oval line end type. |
| ArrowOpen | `5` | Arrow Open line end type. |

### Examples

```csharp
// Called: line.BeginType = MsoArrowheadStyle.Arrow;
public static void Type_MsoArrowheadStyle()
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

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


