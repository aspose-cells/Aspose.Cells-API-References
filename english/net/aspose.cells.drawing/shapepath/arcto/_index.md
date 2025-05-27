---
title: ShapePath.ArcTo
second_title: Aspose.Cells for .NET API Reference
description: ShapePath method. Appends an elliptical arc to the current figure. The starting point is the end point of the current figure
type: docs
url: /net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

Appends an elliptical arc to the current figure. The starting point is the end point of the current figure.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| Parameter | Type | Description |
| --- | --- | --- |
| wR | Single | The half-width of the rectangular area of ​​the ellipse that draws the arc. |
| hR | Single | The half-height of the rectangular area of ​​the ellipse that draws the arc. |
| stAng | Single | The starting angle of the arc, measured in degrees clockwise from the x-axis. |
| swAng | Single | The angle between startAngle and the end of the arc. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to the worksheet
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 200, 0, 0);
            
            // Get the shape's path
            ShapePath shapePath = new ShapePath();
            
            try
            {
                // Move to starting point
                shapePath.MoveTo(50, 50);
                
                // Call ArcTo with parameters: (widthRadius, heightRadius, startAngle, sweepAngle)
                shapePath.ArcTo(30.0f, 20.0f, 0.0f, 90.0f);
                
                // Close the path
                shapePath.Close();
                
                // Set the path to the shape
                var paths = shape.Paths;
                paths.Add();
                
                Console.WriteLine("ArcTo method executed successfully with parameters (Single, Single, Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ArcTo method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


