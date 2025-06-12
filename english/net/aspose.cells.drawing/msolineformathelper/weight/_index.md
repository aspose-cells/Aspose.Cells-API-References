---
title: MsoLineFormatHelper.Weight
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Returns or sets the weight of the line in units of pt
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/weight/
---
## MsoLineFormatHelper.Weight property

Returns or sets the weight of the line ,in units of pt.

```csharp
public double Weight { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyWeightDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to demonstrate MsoLineFormatHelper
            var line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);
            
            // Get the MsoLineFormat for the line
            MsoLineFormat lineFormat = line.LineFormat;

            // Display the current weight value
            Console.WriteLine("Current line weight: " + lineFormat.Weight + " pt");

            // Change the line weight to 3 pt (thicker line)
            lineFormat.Weight = 3.0;

            // Change line color to blue for better visibility
            lineFormat.ForeColor = System.Drawing.Color.Blue;

            // Add another line with default weight for comparison
            var line2 = worksheet.Shapes.AddLine(5, 15, 100, 15, 10, 100);
            line2.LineFormat.ForeColor = System.Drawing.Color.Red;

            // Save the workbook to show the difference
            workbook.Save("LineWeightDemo.xlsx");

            Console.WriteLine("Line weight demonstration completed. Check LineWeightDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


