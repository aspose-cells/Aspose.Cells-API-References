---
title: Line.Transparency
second_title: Aspose.Cells for .NET API Reference
description: Line property. Returns or sets the degree of transparency of the line as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyTransparencyDemo
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
                // Add a line chart to demonstrate line properties
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Get the line properties from the chart series border
                Line line = chart.NSeries[0].Border;

                // Display the current Transparency value
                Console.WriteLine("Current Transparency: " + line.Transparency);

                // Set a new Transparency value (0.0 = opaque, 1.0 = clear)
                line.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + line.Transparency);

                // Save the workbook
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("Transparency property demonstrated successfully.");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


