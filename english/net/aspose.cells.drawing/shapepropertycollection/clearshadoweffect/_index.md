---
title: ShapePropertyCollection.ClearShadowEffect
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection method. Clears the shadow effect of the chart element or shape
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/clearshadoweffect/
---
## ShapePropertyCollection.ClearShadowEffect method

Clears the shadow effect of the chart element or shape.

```csharp
public void ClearShadowEffect()
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapePropertyCollectionMethodClearShadowEffectDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyCollectionMethodClearShadowEffectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape with shadow effect
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.ShadowEffect.Angle = 45;
            shape.ShadowEffect.Distance = 10;
            shape.ShadowEffect.Blur = 5;
            shape.ShadowEffect.Transparency = 0.5;

            try
            {
                // Check if shape has shadow effect before clearing
                bool hasShadowBefore = shape.ShadowEffect != null && shape.ShadowEffect.Distance > 0;
                Console.WriteLine($"Shape has shadow effect before clearing: {hasShadowBefore}");

                // Clear the shadow effect by resetting its properties
                shape.ShadowEffect.Angle = 0;
                shape.ShadowEffect.Distance = 0;
                shape.ShadowEffect.Blur = 0;
                shape.ShadowEffect.Transparency = 0;

                // Verify shadow effect was cleared
                bool hasShadowAfter = shape.ShadowEffect != null && shape.ShadowEffect.Distance > 0;
                Console.WriteLine($"Shape has shadow effect after clearing: {hasShadowAfter}");

                // Additional verification by checking shadow properties
                if (shape.ShadowEffect.Distance == 0 && shape.ShadowEffect.Blur == 0)
                {
                    Console.WriteLine("Shadow effect successfully cleared");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearShadowEffect method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodClearShadowEffectDemo.xlsx");
        }
    }
}
```

### See Also

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


