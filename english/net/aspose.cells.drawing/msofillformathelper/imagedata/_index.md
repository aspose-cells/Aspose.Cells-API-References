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
    using System.IO;

    public class MsoFillFormatHelperPropertyImageDataDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to access MsoFillFormat
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Get the fill format
            MsoFillFormat fillFormat = shape.FillFormat;

            // Display current ImageData (should be null initially)
            Console.WriteLine("Current ImageData is null: " + (fillFormat.ImageData == null));

            // Load an image file for the fill
            byte[] imageData = File.ReadAllBytes("example.jpg");
            fillFormat.ImageData = imageData;

            // Verify the image was set
            Console.WriteLine("ImageData after setting: " + (fillFormat.ImageData != null));

            // Create another shape to demonstrate different fill
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 100, 100, 100);
            MsoFillFormat fillFormat2 = shape2.FillFormat;

            // Set gradient fill for comparison
            fillFormat2.SetOneColorGradient(System.Drawing.Color.Blue, 0.5, GradientStyleType.Horizontal, 1);

            // Save the workbook to show both fill types
            workbook.Save("PropertyImageDataDemo.xlsx");
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


