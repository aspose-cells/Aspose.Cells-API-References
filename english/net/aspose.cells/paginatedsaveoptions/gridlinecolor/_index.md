---
title: PaginatedSaveOptions.GridlineColor
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Gets or sets gridline color
type: docs
url: /net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

Gets or sets gridline color.

```csharp
public Color GridlineColor { get; set; }
```

### Remarks

It will ignore the gridline color settings in the source file.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Create PDF save options
                PdfSaveOptions options = new PdfSaveOptions();

                // Display the default GridlineColor value
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // Set a new gridline color
                options.GridlineColor = Color.Red;

                // Display the updated GridlineColor value
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // Save the workbook with the gridline color setting
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


