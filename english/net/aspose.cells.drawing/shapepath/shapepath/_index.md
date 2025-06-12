---
title: ShapePath.ShapePath
second_title: Aspose.Cells for .NET API Reference
description: ShapePath constructor. Initializes a new instance of the ShapePath class
type: docs
url: /net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

Initializes a new instance of the [`ShapePath`](../) class.

```csharp
public ShapePath()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a new shape path using the #ctor method
                ShapePath shapePath = new ShapePath();

                // Add path segments to create a simple shape
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                // Create a shape and add the path
                var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 300, 300, 0, 0);
                var paths = shape.Paths;
                paths.Add();

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // Save the result
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


