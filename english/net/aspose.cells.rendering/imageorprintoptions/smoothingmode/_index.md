---
title: ImageOrPrintOptions.SmoothingMode
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Specifies whether smoothing antialiasing is applied to lines and curves and the edges of filled areas. The default value is SmoothingMode.None
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Specifies whether smoothing (antialiasing) is applied to lines and curves and the edges of filled areas. The default value is SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySmoothingModeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Create ImageOrPrintOptions instance
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Display some of the available properties
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // Create a SheetRender to demonstrate the property
                SheetRender renderer = new SheetRender(worksheet, options);

                // Render to a memory stream to demonstrate functionality
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Save the workbook
                workbook.Save("ImageOrPrintOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


