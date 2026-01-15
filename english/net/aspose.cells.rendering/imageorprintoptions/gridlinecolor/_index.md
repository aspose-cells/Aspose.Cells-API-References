---
title: ImageOrPrintOptions.GridlineColor
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets gridline colr
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Gets or sets gridline colr.

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
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Put some sample data so that the worksheet has content
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // Create an instance of ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Display the current GridlineColor value (read‑only or read/write)
                // The property type is assumed to be System.Drawing.Color
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // Optionally render the sheet to an image to see the effect of the default gridline color
                // (No need to change the value; we just demonstrate usage.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // Save the workbook (optional)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


