---
title: "TextureFill.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextureFill-egenskap. Hämtar och anger texturtypen"
type: docs
url: /sv/net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Hämtar och anger texturtypen

```csharp
public TextureType Type { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform för att demonstrera texturfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Ställ in fyllningstyp till textur
            shape.Fill.FillType = FillType.Texture;

            // Kom åt egenskaperna för texturfyllning
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // Visa det ursprungliga Type-värdet
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // Ange en annan texturtyp
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // Demonstrera en annan texturtyp
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // Spara arbetsboken för att se effekten
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

### Se även

* enum [TextureType](../../texturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


