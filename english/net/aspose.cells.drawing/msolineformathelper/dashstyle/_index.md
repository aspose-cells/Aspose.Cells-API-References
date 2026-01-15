---
title: MsoLineFormatHelper.DashStyle
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Gets or sets the dash style for the specified line
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

Gets or sets the dash style for the specified line.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyDashStyleDemo
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

                // Display the current DashStyle value
                Console.WriteLine("Current DashStyle: " + lineFormat.DashStyle);

                // Set a new DashStyle value (since it's read/write)
                lineFormat.DashStyle = MsoLineDashStyle.DashDot;
                Console.WriteLine("Updated DashStyle: " + lineFormat.DashStyle);

                // Show how the property affects behavior
                Console.WriteLine("Line dash style has been updated to: " + lineFormat.DashStyle);

                // Save the result
                workbook.Save("DashStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line dash style.");
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

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


