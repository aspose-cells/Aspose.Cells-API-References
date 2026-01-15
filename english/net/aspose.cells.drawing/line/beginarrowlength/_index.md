---
title: Line.BeginArrowLength
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the length of the arrowhead for the begin of a line
type: docs
url: /net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Specifies the length of the arrowhead for the begin of a line.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare simple data for a chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Add a line chart
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Access the line (border) of the first series
                Line seriesLine = chart.NSeries[0].Border;

                // Set the BeginArrowLength to Long
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // Read and display the current BeginArrowLength value
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // Save the workbook (optional, just to complete the demo)
                workbook.Save("BeginArrowLengthDemo.xlsx");
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


