---
title: ShapePropertyCollection.GlowEffect
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection property. Represents a GlowEffect object that specifies glow effect for the chart element or shape
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/gloweffect/
---
## ShapePropertyCollection.GlowEffect property

Represents a `GlowEffect` object that specifies glow effect for the chart element or shape.

```csharp
public GlowEffect GlowEffect { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ShapePropertyCollectionPropertyGlowEffectDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyCollectionPropertyGlowEffectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape to the worksheet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            try
            {
                // Access the GlowEffect property (read-only)
                GlowEffect glowEffect = shape.Glow;

                // Display glow effect properties if it exists
                if (glowEffect != null)
                {
                    Console.WriteLine("Glow Effect Properties:");
                    Console.WriteLine($"Color: {glowEffect.Color}");
                    Console.WriteLine($"Size: {glowEffect.Size}");
                    Console.WriteLine($"Transparency: {glowEffect.Transparency}");
                }
                else
                {
                    Console.WriteLine("No glow effect is currently applied");
                }

                // Demonstrate checking if shape has glow effect
                bool hasGlow = shape.Glow != null;
                Console.WriteLine($"Shape has glow effect: {hasGlow}");

                // Save the workbook
                workbook.Save("GlowEffectDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [GlowEffect](../../gloweffect/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


