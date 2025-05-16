---
title: ShapePropertyCollection.ClearGlowEffect
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection method. Clears the glow effect of the shape
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/cleargloweffect/
---
## ShapePropertyCollection.ClearGlowEffect method

Clears the glow effect of the shape.

```csharp
public void ClearGlowEffect()
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapePropertyCollectionMethodClearGlowEffectDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyCollectionMethodClearGlowEffectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with glow effect
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Glow.Size = 10;
            shape.Glow.Transparency = 0.5;

            try
            {
                // Check if shape has glow effect before clearing
                bool hasGlowBefore = shape.Glow != null && shape.Glow.Size > 0;
                Console.WriteLine($"Shape has glow effect before clearing: {hasGlowBefore}");

                // Clear the glow effect by setting size to 0
                shape.Glow.Size = 0;

                // Verify glow effect was cleared
                bool hasGlowAfter = shape.Glow != null && shape.Glow.Size > 0;
                Console.WriteLine($"Shape has glow effect after clearing: {hasGlowAfter}");

                if (!hasGlowAfter)
                {
                    Console.WriteLine("Glow effect successfully cleared");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearGlowEffect method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodClearGlowEffectDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


