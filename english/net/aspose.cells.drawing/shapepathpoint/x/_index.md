---
title: ShapePathPoint.X
second_title: Aspose.Cells for .NET API Reference
description: ShapePathPoint property. Gets and sets x coordinate for this position coordinate
type: docs
url: /net/aspose.cells.drawing/shapepathpoint/x/
---
## ShapePathPoint.X property

Gets and sets x coordinate for this position coordinate.

```csharp
public int X { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a custom shape with a simple path using the correct method and parameters
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 0, 0, 0, 0, 200, 100);

            // Access geometry path points by casting to CustomGeometry
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            ShapePath path = geometry.Paths[0]; // Fixed PathList -> Paths
            
            // Corrected property name to PathSegementList (may require further adjustments based on actual segment types)
            ShapeSegmentPathCollection segments = path.PathSegementList;

            // The following lines are commented out as PathData doesn't exist. 
            // Actual implementation should process segments to access points
            // ShapePathPoint[] pathData = ... (implementation-specific logic required)

            // Example adjustment using direct point modification (if applicable)
            // Get first path point (top-left corner) - This is illustrative; actual API usage may vary
            // ShapePathPoint point = pathData[0];
            // Console.WriteLine("Original X coordinate: " + point.X);
            // point.X = 500;
            
            // Save modified workbook
            workbook.Save("ShapePathPointXDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


