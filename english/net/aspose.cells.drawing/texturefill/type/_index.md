---
title: TextureFill.Type
second_title: Aspose.Cells for .NET API Reference
description: TextureFill property. Gets and sets the texture type
type: docs
url: /net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Gets and sets the texture type

```csharp
public TextureType Type { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a rectangle shape to demonstrate texture fill
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Set fill type to texture
            shape.Fill.FillType = FillType.Texture;

            // Access the texture fill properties
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // Display the initial Type value
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // Set a different texture type
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // Demonstrate another texture type
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // Save the workbook to see the effect
                workbook.Save("TextureFillTypeDemo.xlsx");
                Console.WriteLine("Texture fill type demonstration completed successfully.");
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

* enum [TextureType](../../texturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


