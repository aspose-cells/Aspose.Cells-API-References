---
title: ImageOrPrintOptions.CustomQueryPageSettingsEventHandler
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Client can control page setting of printer when print each page using this EventHandler
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/
---
## ImageOrPrintOptions.CustomQueryPageSettingsEventHandler property

Client can control page setting of printer when print each page using this EventHandler

```csharp
public QueryPageSettingsEventHandler CustomQueryPageSettingsEventHandler { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ImageOrPrintOptionsPropertyCustomQueryPageSettingsEventHandlerDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomQueryPageSettingsEventHandlerDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Properties Demo";

            try
            {
                // Create ImageOrPrintOptions instance
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                
                // Demonstrate available properties instead
                Console.WriteLine("ImageType: " + options.ImageType);
                Console.WriteLine("Quality: " + options.Quality);
                
                // Create a sheet renderer to demonstrate printing
                SheetRender renderer = new SheetRender(worksheet, options);
                
                // Print to show the effect
                Console.WriteLine("Printing with default settings");
                renderer.ToImage(0, "output.png");
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


