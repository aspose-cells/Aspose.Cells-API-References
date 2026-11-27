---
title: "Enum PresetShadowType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.PresetShadowType‑enum. Representerar förinställd skuggtyp"
type: docs
url: /sv/net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

Representerar förinställd skuggtyp.

```csharp
public enum PresetShadowType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| NoShadow | `0` | Ingen skugga. |
| Custom | `1` | Anpassad skugga. |
| OffsetDiagonalBottomRight | `2` | Yttre skuggförskjutning diagonal nedre högra. |
| OffsetBottom | `3` | Yttre skuggförskjutning nedåt. |
| OffsetDiagonalBottomLeft | `4` | Yttre skuggförskjutning diagonal nedre vänstra. |
| OffsetRight | `5` | Yttre skuggförskjutning åt höger. |
| OffsetCenter | `6` | Yttre skuggförskjutning centrerad. |
| OffsetLeft | `7` | Yttre skuggförskjutning åt vänster. |
| OffsetDiagonalTopRight | `8` | Yttre skuggförskjutning diagonal övre högra. |
| OffsetTop | `9` | Yttre skuggförskjutning uppåt. |
| OffsetDiagonalTopLeft | `10` | Yttre skuggförskjutning diagonal övre vänstra. |
| InsideDiagonalTopLeft | `11` | Inre skugga inuti diagonal övre vänster. |
| InsideTop | `12` | Inre skugga inuti toppen. |
| InsideDiagonalTopRight | `13` | Inre skugga inuti diagonal övre högra. |
| InsideLeft | `14` | Inre skugga inuti vänster. |
| InsideCenter | `15` | Inre skugga i mitten. |
| InsideRight | `16` | Inre skugga till höger. |
| InsideDiagonalBottomLeft | `17` | Inre skugga i diagonal nedre vänster. |
| InsideBottom | `18` | Inre skugga längst ner. |
| InsideDiagonalBottomRight | `19` | Inre skugga i diagonal nedre höger. |
| PerspectiveDiagonalUpperLeft | `20` | Yttre skugga perspektiv diagonal övre vänster. |
| PerspectiveDiagonalUpperRight | `21` | Yttre skugga perspektiv diagonal övre höger. |
| Below | `22` | Yttre skugga nedanför. |
| PerspectiveDiagonalLowerLeft | `23` | Yttre skugga perspektiv diagonal nedre vänster. |
| PerspectiveDiagonalLowerRight | `24` | Yttre skugga perspektiv diagonal nedre höger. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetShadowTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera skuggeffekter
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Ställ in olika förinställda skuggtyper
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
            Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);

            // Byt till en annan skuggtyp
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
            Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);

            // Spara arbetsboken
            workbook.Save("PresetShadowTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


