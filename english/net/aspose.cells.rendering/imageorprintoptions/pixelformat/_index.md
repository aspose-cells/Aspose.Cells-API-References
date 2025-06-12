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
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PixelFormat Demo");
            
            // Create image or print options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Create sheet render and save to image
            SheetRender render = new SheetRender(worksheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                render.ToImage(0, stream);
                
                // Verify the image format
                stream.Position = 0;
                Console.WriteLine($"Image saved successfully");
            }
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


