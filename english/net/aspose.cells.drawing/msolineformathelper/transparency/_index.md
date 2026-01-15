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

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Create a shape to demonstrate line formatting
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Get the line format
                MsoLineFormat lineFormat = shape.LineFormat;

                // Display the current Transparency value
                Console.WriteLine("Current Transparency: " + lineFormat.Transparency);

                // Set a new Transparency value (since it's read/write)
                lineFormat.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + lineFormat.Transparency);

                // Show how the property affects behavior
                Console.WriteLine("Line transparency has been updated to: " + lineFormat.Transparency);

                // Save the result
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line transparency.");
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

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


