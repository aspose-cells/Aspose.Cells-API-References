---
title: ShapePath.CubicBezierTo
second_title: Aspose.Cells for .NET API Reference
description: ShapePath method. Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure
type: docs
url: /net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ctrX1 | Single | The x-coordinate of the first control point for the curve. |
| ctrY1 | Single | The y-coordinate of the first control point for the curve. |
| ctrX2 | Single | The x-coordinate of the second control point for the curve. |
| ctrY2 | Single | The y-coordinate of the second control point for the curve. |
| endX | Single | The x-coordinate of the endpoint of the curve. |
| endY | Single | The y-coordinate of the endpoint of the curve. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to the worksheet
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 200, 200, 200);
            
            // Get the shape's path
            ShapePathCollection shapePaths = shape.Paths;
            ShapePath shapePath = shapePaths[0];
            
            try
            {
                // Move to starting point
                shapePath.MoveTo(10f, 10f);
                
                // Draw a cubic bezier curve with control points (30,30), (50,50) and end point (100,100)
                shapePath.CubicBezierTo(30f, 30f, 50f, 50f, 100f, 100f);
                
                // No need to assign back as we modified the existing path collection
                Console.WriteLine("CubicBezierTo method executed successfully with parameters (Single, Single, Single, Single, Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CubicBezierTo method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


