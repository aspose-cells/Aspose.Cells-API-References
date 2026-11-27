---
title: "Enum PresetWordArtStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.PresetWordArtStyle enum. Representerar de förinställda WordArt-stilarna"
type: docs
url: /sv/net/aspose.cells.drawing/presetwordartstyle/
---
## PresetWordArtStyle enumeration

Representerar de förinställda WordArt-stilarna.

```csharp
public enum PresetWordArtStyle
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| WordArtStyle1 | `1` | Fyll - Svart, Text 1, Skugga |
| WordArtStyle2 | `2` | Fyll - Blå, Accent 1, Skugga |
| WordArtStyle3 | `3` | Fyll - Orange, Accent 2, Kontur - Accent 2 |
| WordArtStyle4 | `4` | Fyll - Vit, Kontur - Accent 1, Skugga |
| WordArtStyle5 | `5` | Fyll - Guld, Accent 4, Mjuk avfasning |
| WordArtStyle6 | `6` | Gradientfyllning - Grå |
| WordArtStyle7 | `7` | Gradientfyllning - Blå, Accent 1, Reflektion |
| WordArtStyle8 | `8` | Gradientfyllning - Guld, Accent 4, Kontur - Accent 4 |
| WordArtStyle9 | `9` | Fyll - Vit, Kontur - Accent 1, Glöd - Accent 1 |
| WordArtStyle10 | `10` | Fyll - Grå-50%, Accent 3, Skarp avfasning |
| WordArtStyle11 | `11` | Fyll - Svart, Text 1, Kontur - Bakgrund 1, Hård skugga - Bakgrund 1 |
| WordArtStyle12 | `12` | Fyll - Svart, Text 1, Kontur - Bakgrund 1, Hård skugga - Accent 1 |
| WordArtStyle13 | `13` | Fyll - Blå, Accent 1, Kontur - Bakgrund 1, Hård skugga - Accent 1 |
| WordArtStyle14 | `14` | Fyll - Vit, Kontur - Accent 2, Hård skugga - Accent 2 |
| WordArtStyle15 | `15` | Fyll - Grå-25%, Bakgrund 2, Inre skugga |
| WordArtStyle16 | `16` | Mönsterfyllning - Vit, Text 2, Mörk uppåtriktad diagonal, Skugga |
| WordArtStyle17 | `17` | Mönsterfyllning - Grå-50%, Accent 3, Smal horisontell, Inre skugga |
| WordArtStyle18 | `18` | Fyll - Blå, Accent 1, 50%, Hård skugga - Accent 1 |
| WordArtStyle19 | `19` | Mönsterfyllning - Blå, Accent 1, Ljus nedåtriktad diagonal, Kontur - Accent 1 |
| WordArtStyle20 | `20` | Mönsterfyllning - Blå-grå, Text 2, Mörk uppåtriktad diagonal, Hård skugga - Text 2 |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PresetWordArtStyleDemo
    {
        public static void PresetWordArtStyleExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Få åtkomst till formsamlingen i kalkylbladet
            ShapeCollection shapes = worksheet.Shapes;
            
            // Lägg till en WordArt-form med en specifik förinställd stil
            // Parametrar: style, text, upperLeftRow, top, upperLeftColumn, left, height, width
            Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
            
            // Spara arbetsboken
            workbook.Save("PresetWordArtStyleExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


