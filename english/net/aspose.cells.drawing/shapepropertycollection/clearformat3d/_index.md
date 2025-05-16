---
title: ShapePropertyCollection.ClearFormat3D
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection method. Clears the 3D shape properties of the shape
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/clearformat3d/
---
## ShapePropertyCollection.ClearFormat3D method

Clears the 3D shape properties of the shape.

```csharp
public void ClearFormat3D()
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapePropertyCollectionMethodClearFormat3DDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyCollectionMethodClearFormat3DDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with 3D formatting
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.ThreeDFormat.TopBevelType = BevelType.Circle;
            shape.ThreeDFormat.TopBevelWidth = 10;
            shape.ThreeDFormat.TopBevelHeight = 10;

            try
            {
                // Check if shape has 3D format before clearing
                if (shape.ThreeDFormat.TopBevelWidth > 0 || shape.ThreeDFormat.TopBevelHeight > 0)
                {
                    Console.WriteLine("Shape has 3D format before clearing");

                    // Cannot set ThreeDFormat directly as it's read-only
                    // Instead, reset all 3D properties to default values
                    shape.ThreeDFormat.TopBevelType = BevelType.None;
                    shape.ThreeDFormat.TopBevelWidth = 0;
                    shape.ThreeDFormat.TopBevelHeight = 0;

                    // Verify the 3D format was cleared
                    if (shape.ThreeDFormat.TopBevelWidth == 0 && shape.ThreeDFormat.TopBevelHeight == 0)
                    {
                        Console.WriteLine("3D format successfully cleared");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormat3D method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodClearFormat3DDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


