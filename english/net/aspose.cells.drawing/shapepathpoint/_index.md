---
title: Class ShapePathPoint
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShapePathPoint class. Represents an xy coordinate within the path coordinate space
type: docs
url: /net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

Represents an x-y coordinate within the path coordinate space.

```csharp
public class ShapePathPoint
```

## Properties

| Name | Description |
| --- | --- |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | Gets and sets x coordinate for this position coordinate. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | Gets y coordinate for this position coordinate. |

### Examples

```csharp
namespace AsposeCellsExamples.DrawingClassShapePathPointDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Add a shape that will contain path points with all required parameters
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // Get the geometry path points
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // Access an existing path point (if available)
                    if (path.PathSegementList.Count > 0)
                    {
                        // Get the first point (actual implementation may vary based on segment type)
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // Display the point coordinates
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // Save the workbook
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


