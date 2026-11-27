---
title: "Shape.TextEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Returnerar ett TextEffectFormat-objekt som innehåller texteffektformateringsegenskaper för den angivna formen. Gäller för Shape-objekt som representerar WordArt"
type: docs
url: /sv/net/aspose.cells.drawing/shape/texteffect/
---
## Shape.TextEffect property

Returnerar ett TextEffectFormat-objekt som innehåller formateringsegenskaper för text‑effekter för den angivna formen. Gäller Shape‑objekt som representerar WordArt.

```csharp
public TextEffectFormat TextEffect { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextEffectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en WordArt-form med korrekta parametrar
            Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);

            // Kontrollera om det är WordArt och få åtkomst till TextEffect-egenskaper
            if (shape.IsWordArt)
            {
                TextEffectFormat textEffectFormat = shape.TextEffect;
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = true;
                textEffectFormat.FontName = "Arial";
                textEffectFormat.FontSize = 14;
            }

            // Spara arbetsboken
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


