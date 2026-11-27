---
title: "TextureFill.Scale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextureFill-egenskap. Hämtar och anger skalan för bildformatet"
type: docs
url: /sv/net/aspose.cells.drawing/texturefill/scale/
---
## TextureFill.Scale property

Hämtar och anger skalan för bildformatet.

```csharp
public double Scale { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TextureFillPropertyScaleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form och hämta dess fyllningsformat
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
            FillFormat fillFormat = shape.Fill;

            // Konfigurera texturfyllning
            fillFormat.FillType = FillType.Texture;
            TextureFill textureFill = fillFormat.TextureFill;

            // Läs in texturbild och konfigurera egenskaper
            textureFill.ImageData = File.ReadAllBytes("texture.jpg");
            textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
            textureFill.IsTiling = true;

            // Visa och ändra skala
            Console.WriteLine("Initial Scale: " + textureFill.Scale);
            textureFill.Scale = 0.5;
            Console.WriteLine("Modified Scale: " + textureFill.Scale);

            // Spara resultatet
            workbook.Save("TextureFillScaleDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


