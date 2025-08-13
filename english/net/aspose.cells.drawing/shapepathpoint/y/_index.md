---
title: ShapePathPoint.Y
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPoint property. Gets y coordinate for this position coordinate. Unit EMUs
type: docs
url: /net/aspose.cells.drawing/shapepathpoint/y/
---
## ShapePathPoint.Y property

Gets y coordinate for this position coordinate. Unit EMUs.

```csharp
[Obsolete("Use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Y { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a shape path point collection and add points
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Access points using Item property
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Create a shape path using the points
            ShapePath path = new ShapePath();

            // Move to starting point
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Add freeform shape with the configured path
            Shape shape = worksheet.Shapes.AddFreeform(
                    upperLeftRow: 2,
                    top: 0,
                    upperLeftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Save the modified workbook
            workbook.Save("ShapePathPointYDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


