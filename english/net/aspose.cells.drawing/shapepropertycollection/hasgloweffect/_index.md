---
title: ShapePropertyCollection.HasGlowEffect
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection method. Indicates if the shape has glow effect data
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/hasgloweffect/
---
## ShapePropertyCollection.HasGlowEffect method

Indicates if the shape has glow effect data.

```csharp
public bool HasGlowEffect()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyCollectionMethodHasGlowEffectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to test glow effects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // Check if shape has glow effect before any modifications
                bool hasGlowBefore = shape.Glow != null && shape.Glow.Size > 0;
                Console.WriteLine($"Shape has glow effect before: {hasGlowBefore}");

                // Apply glow effect
                shape.Glow.Size = 10;
                shape.Glow.Transparency = 0.5;

                // Check if shape has glow effect after modification
                bool hasGlowAfter = shape.Glow != null && shape.Glow.Size > 0;
                Console.WriteLine($"Shape has glow effect after: {hasGlowAfter}");

                // Clear glow effect by setting size to 0
                shape.Glow.Size = 0;

                // Verify glow effect is cleared
                bool hasGlowCleared = shape.Glow != null && shape.Glow.Size > 0;
                Console.WriteLine($"Shape has glow effect after clear: {hasGlowCleared}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HasGlowEffect method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodHasGlowEffectDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


