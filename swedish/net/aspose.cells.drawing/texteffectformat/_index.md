---
title: "Klass TextEffectFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.TextEffectFormat-klass. Innehåller egenskaper och metoder som gäller för WordArt-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/
---
## TextEffectFormat class

Innehåller egenskaper och metoder som gäller för WordArt‑objekt.

```csharp
public class TextEffectFormat
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | Anger om teckensnittet är fetstil. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | Anger om teckensnittet är kursiv. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | Namnet på teckensnittet som används i WordArt. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | Storleken (i punkter) på teckensnittet som används i WordArt. |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | Hämtar och anger den förinställda formtypen. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | Om sant roteras tecknen i den angivna WordArt med 90 grader i förhållande till WordArts omgivande form. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | Texten i WordArt. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | Anger den förinställda texteffekten. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextEffectFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            
            // Lägg till texteffektform
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            
            // Modifiera texteffekt
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;
            textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
            
            // Spara arbetsboken
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


