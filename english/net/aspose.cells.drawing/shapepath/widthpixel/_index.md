---
title: ShapePath.WidthPixel
second_title: Aspose.Cells for .NET API Reference
description: ShapePath property. Gets the width of this path in unit of pixels
type: docs
url: /net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

Gets the width of this path in unit of pixels.

```csharp
public int WidthPixel { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // Display the initial WidthPixel value
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // Set a new width value
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // Add the shape to the worksheet
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // Save the workbook
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


