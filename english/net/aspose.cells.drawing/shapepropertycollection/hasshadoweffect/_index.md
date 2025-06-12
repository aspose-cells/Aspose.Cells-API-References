---
title: ShapePropertyCollection.HasShadowEffect
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection method. Indicates if the shape has shadow effect data
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/hasshadoweffect/
---
## ShapePropertyCollection.HasShadowEffect method

Indicates if the shape has shadow effect data.

```csharp
public bool HasShadowEffect()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyCollectionMethodHasShadowEffectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to test shadow effects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // Check if shape has shadow effect before any modifications
                bool hasShadowBefore = shape.ShadowEffect != null;
                Console.WriteLine($"Shape has shadow effect before: {hasShadowBefore}");

                // Apply shadow effect
                shape.ShadowEffect.Angle = 45;
                shape.ShadowEffect.Size = 10;
                shape.ShadowEffect.Distance = 10;
                shape.ShadowEffect.Blur = 5;
                shape.ShadowEffect.Transparency = 0.5;

                // Check if shape has shadow effect after modification
                bool hasShadowAfter = shape.ShadowEffect != null;
                Console.WriteLine($"Shape has shadow effect after: {hasShadowAfter}");

                // Clear shadow effect by setting properties to default/empty values
                shape.ShadowEffect.Angle = 0;
                shape.ShadowEffect.Size = 0;
                shape.ShadowEffect.Distance = 0;
                shape.ShadowEffect.Blur = 0;
                shape.ShadowEffect.Transparency = 0;

                // Verify shadow effect is cleared
                bool hasShadowCleared = shape.ShadowEffect.Size == 0 && shape.ShadowEffect.Distance == 0;
                Console.WriteLine($"Shape has shadow effect after clear: {hasShadowCleared}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HasShadowEffect method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodHasShadowEffectDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


