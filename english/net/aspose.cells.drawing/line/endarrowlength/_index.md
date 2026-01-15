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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyEndArrowLengthDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Add a chart to demonstrate line properties
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Get the line properties from the chart series border
                Line line = chart.NSeries[0].Border;

                // Set an arrowhead type to demonstrate EndArrowLength
                line.EndType = MsoArrowheadStyle.Arrow;

                // Display the current EndArrowLength value
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // Set a new EndArrowLength value
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // Save the workbook
                workbook.Save("EndArrowLengthDemo.xlsx");
                Console.WriteLine("EndArrowLength property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


