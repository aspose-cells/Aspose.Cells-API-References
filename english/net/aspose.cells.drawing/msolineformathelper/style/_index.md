---
title: MsoLineFormatHelper.Style
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Returns a Style object that represents the style of the specified range
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

Returns a Style object that represents the style of the specified range.

```csharp
public MsoLineStyle Style { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
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

                // Get the line format directly (MsoLineFormatHelper appears to be a helper class)
                // Since we can't instantiate MsoLineFormatHelper directly, we'll work with the LineFormat property
                MsoLineFormat lineFormat = shape.LineFormat;

                // Display the current Style value
                Console.WriteLine("Current Line Style: " + lineFormat.Style);

                // Set a new style (since Style is read/write)
                lineFormat.Style = MsoLineStyle.ThickBetweenThin;
                Console.WriteLine("Updated Line Style: " + lineFormat.Style);

                // Show how the property affects behavior
                Console.WriteLine("Line style has been updated to: " + lineFormat.Style);

                // Save the result
                workbook.Save("LineStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line style.");
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

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


