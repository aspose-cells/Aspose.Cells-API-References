---
title: "TextureFill.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextureFill-egenskap. Returnerar eller anger transparensgraden för området som ett värde från 0.0 ogenomskinligt till 1.0 helt genomskinligt"
type: docs
url: /sv/net/aspose.cells.drawing/texturefill/transparency/
---
## TextureFill.Transparency property

Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform i arbetsbladet
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Ställ in fyllningstyp till textur
            shape.Fill.FillType = FillType.Texture;

            // Kom åt egenskaperna för texturfyllning
            TextureFill textureFill = shape.Fill.TextureFill;

            // Ange en inbyggd texturtyp
            textureFill.Type = TextureType.BlueTissuePaper;

            // Visa initialt transparensvärde
            Console.WriteLine("Initial Transparency: " + textureFill.Transparency);

            // Ändra transparensen till 70 % (0.0 = ogenomskinlig, 1.0 = helt genomskinlig)
            textureFill.Transparency = 0.7;
            Console.WriteLine("Updated Transparency: " + textureFill.Transparency);

            // Spara arbetsboken med synligt transparenseffekt
            workbook.Save("TextureFillTransparencyDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


