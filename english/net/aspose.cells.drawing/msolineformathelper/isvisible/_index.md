---
title: MsoLineFormatHelper.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormatHelper property. Indicates whether the object is visible
type: docs
url: /net/aspose.cells.drawing/msolineformathelper/isvisible/
---
## MsoLineFormatHelper.IsVisible property

Indicates whether the object is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyIsVisibleDemo
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

                // Display the current IsVisible value
                Console.WriteLine("Current IsVisible: " + lineFormat.IsVisible);

                // Set a new IsVisible value (since it's read/write)
                lineFormat.IsVisible = false;
                Console.WriteLine("Updated IsVisible: " + lineFormat.IsVisible);

                // Show how the property affects behavior
                Console.WriteLine("Line visibility has been updated to: " + lineFormat.IsVisible);

                // Save the result
                workbook.Save("IsVisibleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line visibility.");
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


