---
title: Line.EndArrowLength
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the length of the arrowhead for the end of a line
type: docs
url: /net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Specifies the length of the arrowhead for the end of a line.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);
public static void Property_EndArrowLength()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Create a line shape for the chart
            Line line = chart.Line;

            // Set the arrowhead lengths
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // Output the arrowhead lengths
            Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowLength);
            Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);

            // Save the workbook
            workbook.Save("MsoArrowheadLengthExample.xlsx");
        }
```

### See Also

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


