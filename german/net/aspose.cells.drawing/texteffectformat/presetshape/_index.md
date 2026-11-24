---
title: "TextEffectFormat.PresetShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextEffectFormat-Eigenschaft. Ruft den voreingestellten Formtyp ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

Liest und setzt den voreingestellten Formtyp.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyPresetShapeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form mit Texteffekt hinzu
            Shape shape = worksheet.Shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect1,
                "Sample Text",
                "Arial",
                18,
                false,
                false,
                0,
                0,
                100,
                200,
                0,
                0);

            // Erhalte das TextEffectFormat
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Setze und rufe die PresetShape-Eigenschaft ab
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
            Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);

            // Andere Eigenschaften ändern
            textEffectFormat.Text = "Updated Text";
            textEffectFormat.FontBold = true;
            textEffectFormat.FontSize = 24;

            // Speichere die Arbeitsmappe
            workbook.Save("TextEffectFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


