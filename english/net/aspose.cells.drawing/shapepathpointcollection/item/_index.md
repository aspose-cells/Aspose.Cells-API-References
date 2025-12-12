---
title: ShapePathPointCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPointCollection property. Gets shape path point by index
type: docs
url: /net/aspose.cells.drawing/shapepathpointcollection/item/
---
## ShapePathPointCollection indexer

Gets shape path point by index.

```csharp
public ShapePathPoint this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index |

### Return Value

Returns [`ShapePathPoint`](../../shapepathpoint/) object

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionPropertyItemDemo
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
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Save the result
            workbook.Save("ShapePathPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePathPoint](../../shapepathpoint/)
* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


