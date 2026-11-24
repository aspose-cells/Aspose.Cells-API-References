---
title: "Klasse TextEffectFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.TextEffectFormat Klasse. Enthält Eigenschaften und Methoden, die auf WordArt‑Objekte angewendet werden"
type: docs
url: /de/net/aspose.cells.drawing/texteffectformat/
---
## TextEffectFormat class

Enthält Eigenschaften und Methoden, die auf WordArt-Objekte angewendet werden.

```csharp
public class TextEffectFormat
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | Gibt an, ob die Schrift fett ist. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | Gibt an, ob die Schrift kursiv ist. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | Der Name der im WordArt verwendeten Schrift. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | Die Größe (in Punkten) der im WordArt verwendeten Schrift. |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | Liest und setzt den voreingestellten Formtyp. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | Wenn true, werden die Zeichen im angegebenen WordArt um 90 Grad relativ zur Begrenzungsform des WordArt gedreht. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | Der Text im WordArt. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | Legt den voreingestellten Texteffekt fest. |

### Beispiele

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
            
            // Text‑Effekt‑Form hinzufügen
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            
            // Text‑Effekt ändern
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;
            textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


