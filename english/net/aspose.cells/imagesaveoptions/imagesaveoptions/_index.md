---
title: ImageSaveOptions.ImageSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: ImageSaveOptions constructor. Creates the options for saving image file
type: docs
url: /net/aspose.cells/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions() {#constructor}

Creates the options for saving image file.

```csharp
public ImageSaveOptions()
```

### Remarks

The default type is Tiff.

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add sample data
            workbook.Worksheets[0].Cells["A1"].PutValue("Sample Image Export");
            
            // Create ImageSaveOptions using constructor
            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            
            // Set image options
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            
            // Save to memory stream
            MemoryStream stream = new MemoryStream();
            workbook.Save(stream, pngOptions);
            
            // Verify the output (PNG magic number)
            Console.WriteLine("First byte of PNG: 0x{0:X2}", stream.GetBuffer()[0]);
        }
    }
}
```

### See Also

* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImageSaveOptions(SaveFormat) {#constructor_1}

Creates the options for saving image file.

```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Tiff, Svg, Bmp, Png, Jpg, Emf or Gif, otherwise the saved format will be set as Tiff automatically. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook and add test data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Save Demo");
            
            // Create ImageSaveOptions with SaveFormat.Tiff
            try
            {
                ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Tiff);
                
                // Configure image rendering options
                saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
                saveOptions.ImageOrPrintOptions.VerticalResolution = 300;

                // Save workbook as multi-page TIFF
                workbook.Save("WorksheetImage.tiff", saveOptions);
                
                Console.WriteLine("Workbook successfully saved as TIFF image with 300 DPI resolution.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image save operation: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


