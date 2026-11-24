---
title: "Enum PresetWordArtStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.PresetWordArtStyle enum. Stellt die vordefinierten WordArt-Stile dar"
type: docs
url: /de/net/aspose.cells.drawing/presetwordartstyle/
---
## PresetWordArtStyle enumeration

Stellt die voreingestellten WordArt‑Stile dar.

```csharp
public enum PresetWordArtStyle
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| WordArtStyle1 | `1` | Füllung - Schwarz, Text 1, Schatten |
| WordArtStyle2 | `2` | Füllung - Blau, Akzent 1, Schatten |
| WordArtStyle3 | `3` | Füllung - Orange, Akzent 2, Kontur - Akzent 2 |
| WordArtStyle4 | `4` | Füllung - Weiß, Kontur - Akzent 1, Schatten |
| WordArtStyle5 | `5` | Füllung - Gold, Akzent 4, Weiche Abschrägung |
| WordArtStyle6 | `6` | Verlaufsfüllung - Grau |
| WordArtStyle7 | `7` | Verlaufsfüllung - Blau, Akzent 1, Spiegelung |
| WordArtStyle8 | `8` | Verlaufsfüllung - Gold, Akzent 4, Kontur - Akzent 4 |
| WordArtStyle9 | `9` | Füllung - Weiß, Kontur - Akzent 1, Leuchten - Akzent 1 |
| WordArtStyle10 | `10` | Füllung - Grau-50%, Akzent 3, Scharfe Abschrägung |
| WordArtStyle11 | `11` | Füllung - Schwarz, Text 1, Kontur - Hintergrund 1, Harter Schatten - Hintergrund 1 |
| WordArtStyle12 | `12` | Füllung - Schwarz, Text 1, Kontur - Hintergrund 1, Harter Schatten - Akzent 1 |
| WordArtStyle13 | `13` | Füllung - Blau, Akzent 1, Kontur - Hintergrund 1, Harter Schatten - Akzent 1 |
| WordArtStyle14 | `14` | Füllung - Weiß, Kontur - Akzent 2, Harter Schatten - Akzent 2 |
| WordArtStyle15 | `15` | Füllung - Grau-25%, Hintergrund 2, Innerer Schatten |
| WordArtStyle16 | `16` | Musterfüllung - Weiß, Text 2, Dunkle Aufwärtsdiagonale, Schatten |
| WordArtStyle17 | `17` | Musterfüllung - Grau-50%, Akzent 3, Schmale Horizontal, Innerer Schatten |
| WordArtStyle18 | `18` | Füllung - Blau, Akzent 1, 50%, Harter Schatten - Akzent 1 |
| WordArtStyle19 | `19` | Musterfüllung - Blau, Akzent 1, Helle Abwärtsdiagonale, Kontur - Akzent 1 |
| WordArtStyle20 | `20` | Musterfüllung - Blau-Grau, Text 2, Dunkle Aufwärtsdiagonale, Harter Schatten - Text 2 |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die Formensammlung des Arbeitsblatts zu
            ShapeCollection shapes = worksheet.Shapes;
            
            // Fügen Sie eine WordArt-Form mit einem bestimmten vordefinierten Stil hinzu
            // Parameter: style, text, upperLeftRow, top, upperLeftColumn, left, height, width
            Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PresetWordArtStyleExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


