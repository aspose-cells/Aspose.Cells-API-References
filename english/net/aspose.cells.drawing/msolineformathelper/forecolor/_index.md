---
title: MsoLineFormatHelper.ForeColor
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Gets and sets the border line fore color
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

Gets and sets the border line fore color.

```csharp
public Color ForeColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyForeColorDemo
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

                // Display the current ForeColor value
                Console.WriteLine("Current ForeColor: " + lineFormat.ForeColor);

                // Set a new ForeColor (since it's read/write)
                lineFormat.ForeColor = Color.Red;
                Console.WriteLine("Updated ForeColor: " + lineFormat.ForeColor);

                // Show how the property affects behavior
                Console.WriteLine("Line fore color has been updated to: " + lineFormat.ForeColor);

                // Save the result
                workbook.Save("ForeColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line fore color.");
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


