---
title: ShadowEffect.Color
second_title: Aspose.Cells for .NET API Reference
description: ShadowEffect property. Gets and sets the color of the shadow
type: docs
url: /net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

Gets and sets the color of the shadow.

```csharp
public CellsColor Color { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape to demonstrate shadow effect
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Get the shadow effect from the shape
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // Create a new CellsColor object
                CellsColor shadowColor = workbook.CreateCellsColor();

                // Set the color to red using RGB values
                shadowColor.Color = Color.Red;

                // Apply the color to the shadow effect
                shadowEffect.Color = shadowColor;

                // Display the current color value
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // Save the workbook to demonstrate the effect
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // Load the workbook back to verify the color was saved
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // Display the loaded color value
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


