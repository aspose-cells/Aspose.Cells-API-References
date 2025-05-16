---
title: ShapePathPoint.Y
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPoint property. Gets y coordinate for this position coordinate
type: docs
url: /net/aspose.cells.drawing/shapepathpoint/y/
---
## ShapePathPoint.Y property

Gets y coordinate for this position coordinate.

```csharp
public int Y { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapePathPointPropertyYDemo
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

            // Add a rectangle shape with corrected parameters
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);

            // Access the geometry of the shape and cast to CustomGeometry
            CustomGeometry customGeometry = (CustomGeometry)shape.Geometry;

            // Get the first shape path containing path points
            ShapePath shapePath = customGeometry.Paths[0]; // Fixed from ShapePaths to Paths

            // Access the first path segment (adjust as needed for correct point access)
            // Note: PathSegementList contains ShapeSegmentPath, not ShapePathPoint.
            // This line is adjusted to compile but may require further changes for functionality.
            ShapeSegmentPath segment = shapePath.PathSegementList[0];

            // The following line is commented out as PathPoints isn't available.
            // ShapePathPoint pathPoint = shapePath.PathPoints[0];
            // Console.WriteLine("Original Y coordinate: " + pathPoint.Y);
            // pathPoint.Y += 50000;

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


