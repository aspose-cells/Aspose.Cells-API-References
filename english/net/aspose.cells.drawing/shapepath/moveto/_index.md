---
title: ShapePath.MoveTo
second_title: Aspose.Cells for .NET API Reference
description: ShapePath method. Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure
type: docs
url: /net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.

```csharp
public void MoveTo(float x, float y)
```

| Parameter | Type | Description |
| --- | --- | --- |
| x | Single | The x-coordinate of the starting point of the figure. |
| y | Single | The y-coordinate of the starting point of the figure. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to the worksheet (fixed by adding height parameter)
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 0, 0, 200, 100, 200, 100);
            
            // Get the shape's geometry path (fixed by using correct property name Paths instead of ShapePaths)
            ShapePath shapePath = ((CustomGeometry)shape.Geometry).Paths[0];

            try
            {
                // Call the MoveTo method with Single parameters
                shapePath.MoveTo(10.5f, 15.5f);
                
                // Add a line from the moved position
                shapePath.LineTo(50.5f, 15.5f);
                
                Console.WriteLine("MoveTo method executed successfully with parameters (10.5f, 15.5f)");
                
                // The shape's path now starts at (10.5, 15.5) and has a line to (50.5, 15.5)
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MoveTo method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


