---
title: "MsoFillFormat.Texture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormat‑egenskap. Hämtar typ av texturfyllning"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Hämtar typen av texturfyllning.

```csharp
public TextureType Texture { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform för att demonstrera fyllningsformatering
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Hämta fyllningsformatet
            MsoFillFormat fillFormat = rectangle.FillFormat;

            try
            {
                // Visa den aktuella texturtypen (skrivskyddad egenskap)
                TextureType currentTexture = fillFormat.Texture;
                Console.WriteLine("Current Texture Type: " + currentTexture);

                // Ange bilddata för att eventuellt ändra texturen
                // Detta demonstrerar hur textur kan påverkas av bilddata
                byte[] sampleImageData = new byte[] { 0x89, 0x50, 0x4E, 0x47 }; // PNG header
                fillFormat.ImageData = sampleImageData;

                // Visa texturtypen igen efter att ha angett bilddata
                TextureType updatedTexture = fillFormat.Texture;
                Console.WriteLine("Texture Type after setting image data: " + updatedTexture);

                // Spara arbetsboken
                workbook.Save("TextureDemo.xlsx");
                Console.WriteLine("Texture demonstration completed successfully.");
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
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


