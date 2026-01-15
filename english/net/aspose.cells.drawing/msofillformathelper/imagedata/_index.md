---
title: MsoFillFormatHelper.ImageData
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Gets and sets the Texture and Picture fill data
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/imagedata/
---
## MsoFillFormatHelper.ImageData property

Gets and sets the Texture and Picture fill data.

```csharp
public byte[] ImageData { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.IO;

    public class MsoFillFormatHelperPropertyImageDataDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a label to make the example meaningful
            worksheet.Cells["A1"].Value = "ImageData Property Demo";

            try
            {
                // Create an instance of MsoFillFormatHelper using reflection (no public constructor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Display the current value of the ImageData property
                Console.WriteLine($"Current ImageData: {(fillHelper.ImageData == null ? "null" : $"Length: {fillHelper.ImageData.Length} bytes")}");

                // Set new image data (create a simple 1x1 pixel red image)
                byte[] imageData = new byte[] { 0x42, 0x4D, 0x3A, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00, 0x28, 0x00,
                                               0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x18, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x00, 0x00, 0x00, 0xFF, 0x00, 0x00 };

                fillHelper.ImageData = imageData;
                Console.WriteLine($"Updated ImageData length: {fillHelper.ImageData.Length} bytes");

                // Demonstrate reading the ImageData value
                byte[] currentImageData = fillHelper.ImageData;
                Console.WriteLine($"Current ImageData length: {currentImageData.Length} bytes");

                // Save the workbook to demonstrate successful execution
                workbook.Save("ImageDataDemo.xlsx");

                Console.WriteLine("ImageData property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ImageData demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


