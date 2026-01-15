---
title: MsoLineFormatHelper.BackColor
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Gets and sets the border line back color
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/backcolor/
---
## MsoLineFormatHelper.BackColor property

Gets and sets the border line back color.

```csharp
public Color BackColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyBackColorDemo
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

                // Display the current BackColor value
                Console.WriteLine("Current BackColor: " + lineFormat.BackColor);

                // Set a new BackColor value (since it's read/write)
                lineFormat.BackColor = Color.LightBlue;
                Console.WriteLine("Updated BackColor: " + lineFormat.BackColor);

                // Show how the property affects behavior
                Console.WriteLine("Line back color has been updated to: " + lineFormat.BackColor);

                // Save the result
                workbook.Save("BackColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line back color.");
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


