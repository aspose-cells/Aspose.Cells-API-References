---
title: "FillFormat.TextureFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Hämtar TextureFill-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/texturefill/
---
## FillFormat.TextureFill property

Hämtar `TextureFill`-objekt.

```csharp
public TextureFill TextureFill { get; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bildform
            string imagePath = Path.Combine("your_image_directory", "texture.png");
            int pictureIndex = worksheet.Pictures.Add(0, 0, imagePath);
            Shape picture = worksheet.Shapes[pictureIndex];

            // Ställ in egenskaper för texturfyllning
            picture.Fill.TextureFill.ImageData = File.ReadAllBytes(imagePath);
            picture.Fill.TextureFill.IsTiling = true;
            picture.Fill.TextureFill.Scale = 0.5;

            // Spara arbetsboken
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


