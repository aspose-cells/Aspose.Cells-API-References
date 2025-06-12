---
title: ShapePath.Close
second_title: Aspose.Cells for .NET API Reference
description: ShapePath method. Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves the method closes the loop by connecting a line from the endpoint to the starting point
type: docs
url: /net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point.

```csharp
public void Close()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a new shape path
                ShapePath shapePath = new ShapePath();

                // Create a simple square path
                shapePath.MoveTo(10.0f, 10.0f);
                shapePath.LineTo(50.0f, 10.0f);
                shapePath.LineTo(50.0f, 50.0f);
                shapePath.LineTo(10.0f, 50.0f);
                
                // Close the path to complete the square
                shapePath.Close();

                // Add the shape to worksheet
                var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 0, 0, 200, 200, 0, 0);
                var paths = shape.Paths;
                paths.Add();

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // Save the workbook
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


