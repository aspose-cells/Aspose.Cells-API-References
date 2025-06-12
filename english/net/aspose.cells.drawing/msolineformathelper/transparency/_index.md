---
title: MsoLineFormatHelper.Transparency
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Returns or sets the degree of transparency of the specified fill as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/transparency/
---
## MsoLineFormatHelper.Transparency property

Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a line shape to demonstrate MsoLineFormat
            var line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);
            MsoLineFormat lineFormat = line.LineFormat;

            // Display current transparency value
            Console.WriteLine("Current Transparency value: " + lineFormat.Transparency);

            // Set different transparency values and observe effects
            lineFormat.Transparency = 0.0; // Opaque
            lineFormat.ForeColor = Color.Red;
            lineFormat.Weight = 5;

            // Add another line with semi-transparent effect
            var line2 = worksheet.Shapes.AddLine(5, 20, 100, 20, 10, 100);
            line2.LineFormat.Transparency = 0.5; // Semi-transparent
            line2.LineFormat.ForeColor = Color.Blue;
            line2.LineFormat.Weight = 5;

            // Add another line with highly transparent effect
            var line3 = worksheet.Shapes.AddLine(5, 35, 100, 35, 10, 100);
            line3.LineFormat.Transparency = 0.8; // Mostly transparent
            line3.LineFormat.ForeColor = Color.Green;
            line3.LineFormat.Weight = 5;

            // Save the workbook to see the transparency effects
            workbook.Save("PropertyTransparencyDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


