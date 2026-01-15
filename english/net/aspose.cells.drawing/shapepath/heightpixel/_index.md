---
title: ShapePath.HeightPixel
second_title: Aspose.Cells for .NET API Reference
description: ShapePath property. Gets the height of this path in unit of pixels
type: docs
url: /net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

Gets the height of this path in unit of pixels.

```csharp
public int HeightPixel { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a new shape path
                ShapePath shapePath = new ShapePath();

                // Create a simple rectangle path
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // Display the current HeightPixel value
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // Set a new height value
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // Add the shape to the worksheet
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // Save the workbook
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
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

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


