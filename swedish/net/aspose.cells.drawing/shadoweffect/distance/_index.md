---
title: "ShadowEffect.Distance"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShadowEffect property. Hämtar och anger avståndet för skuggan. Intervall från 0 till 200 punkter"
type: docs
url: /sv/net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

Hämtar och anger avståndet för skuggan. Intervall från 0 till 200 punkter.

```csharp
public double Distance { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Skapa ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till rektangelform
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
            
            // Konfigurera skuggeffekt
            ShadowEffect shadow = rectangle.ShadowEffect;
            shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
            
            // Skapa CellsColor-objekt och ange ARGB-värden
            CellsColor color = workbook.CreateCellsColor();
            color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
            shadow.Color = color;
            
            shadow.Transparency = 0.3;
            shadow.Blur = 15;
            shadow.Angle = 45;
            shadow.Distance = 20; // Set distance to 20 points

            // Visa skuggavstånd
            Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");

            // Spara arbetsbok med skuggeffekt
            workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


