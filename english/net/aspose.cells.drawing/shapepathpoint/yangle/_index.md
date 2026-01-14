---
title: ShapePathPoint.YAngle
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPoint property. When the object is an angle marker get or set the second angle in degrees
type: docs
url: /net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

When the object is an angle marker, get or set the second angle in degrees.

```csharp
public int YAngle { get; set; }
```

### Remarks

If this angle is the swing angle of an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYAngleDemo
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

                // Add points with angle markers (using XAngle and YAngle)
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // Display the YAngle value
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // Create another point with different angles
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // Display the YAngle value
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // Create a shape path and add arc using angle markers
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

                // Add freeform shape to worksheet
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Save the workbook
                workbook.Save("YAngleDemo.xlsx");
                Console.WriteLine("YAngle property demonstration completed successfully.");
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


