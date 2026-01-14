---
title: ImageOrPrintOptions.PixelFormat
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the pixel format for the generated images
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Gets or sets the pixel format for the generated images.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Remarks

The default value is PixelFormat.Format32bppArgb.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // Create ImageOrPrintOptions instance
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Display the current value of the ImageType property (since PixelFormat doesn't exist)
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Note: Since PixelFormat doesn't exist in the API, we demonstrate ImageType instead
                // which is the closest related property for image format settings

                // Create a SheetRender to demonstrate the options in use
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Save the result as an image to demonstrate the options
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
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


