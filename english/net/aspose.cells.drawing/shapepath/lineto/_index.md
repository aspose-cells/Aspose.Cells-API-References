---
title: ShapePath.LineTo
second_title: Aspose.Cells for .NET API Reference
description: ShapePath method. Appends a line segment to the current figure. The starting point is the end point of the current figure
type: docs
url: /net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

Appends a line segment to the current figure. The starting point is the end point of the current figure.

```csharp
public void LineTo(float x, float y)
```

| Parameter | Type | Description |
| --- | --- | --- |
| x | Single | The x-coordinate of the endpoint of the line segment. |
| y | Single | The y-coordinate of the endpoint of the line segment. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to the worksheet with all required parameters
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 200, 200, 200);
            
            // Get the first path from the shape's paths collection
            ShapePath shapePath = shape.Paths[0];

            try
            {
                // Move to starting point
                shapePath.MoveTo(10, 10);
                
                // Call LineTo method with (Single, Single) parameters
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


