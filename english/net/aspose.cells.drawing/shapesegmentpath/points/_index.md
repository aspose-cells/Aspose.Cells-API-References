---
title: ShapeSegmentPath.Points
second_title: Aspose.Cells for .NET API Reference
description: ShapeSegmentPath property. Gets the points in path segment
type: docs
url: /net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

Gets the points in path segment

```csharp
public ShapePathPointCollection Points { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyPointsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a freeform shape with a custom path
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 400, 400, new ShapePath[] { new ShapePath() });

            // Get the geometry path of the shape
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // Create line segment paths using Add method with LineTo type
            shapePath.PathSegementList.Add(ShapePathType.LineTo);
            shapePath.PathSegementList.Add(ShapePathType.LineTo);

            // Access the first segment path
            ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

            // Display points information
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }

            // Add a new point to the segment (since Points is read-only, we need to modify through the collection)
            ShapePathPointCollection points = segmentPath.Points;
            int newPointIndex = points.Add(150, 150);
            Console.WriteLine($"Added new point at index {newPointIndex}");

            // Display updated points information
            Console.WriteLine("\nUpdated points after addition:");
            for (int i = 0; i < points.Count; i++)
            {
                ShapePathPoint point = points[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Save the workbook
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


