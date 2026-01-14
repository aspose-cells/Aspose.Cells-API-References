---
title: ShapePathPoint.XPixel
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPoint property. When the object is a position coordinate get or set the x coordinate in pixels
type: docs
url: /net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

When the object is a position coordinate, get or set the x coordinate in pixels.

```csharp
public int XPixel { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a shape path point collection
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Add points with coordinates
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // Access the first point and demonstrate XPixel property
                ShapePathPoint firstPoint = pathPoints[0];

                // Display the XPixel value (read operation)
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // Set a new value for XPixel (since it's read/write)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // Create a shape path and add the points
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Add the second point
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

                // Add a freeform shape to the worksheet
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Save the workbook
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
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

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


