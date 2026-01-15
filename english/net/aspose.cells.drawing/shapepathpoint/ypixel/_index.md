---
title: ShapePathPoint.YPixel
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPoint property. When the object is a position coordinate get or set the y coordinate in pixels
type: docs
url: /net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

When the object is a position coordinate, get or set the y coordinate in pixels.

```csharp
public int YPixel { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
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

                // Add a point with coordinates
                pathPoints.Add(100, 50);

                // Access the first point and demonstrate YPixel property
                ShapePathPoint firstPoint = pathPoints[0];

                // Display the initial YPixel value (read operation)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // Set a new value for YPixel (since it's read/write)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // Create a shape path and use the point
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

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
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
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


