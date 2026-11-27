---
title: "TextEffectFormat.PresetShape"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextEffectFormat-egenskap. Hämtar och anger den förinställda formtypen"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

Hämtar och anger den förinställda formtypen.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med texteffekt
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

            // Hämta texteffektformatet
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Ange och hämta PresetShape-egenskapen
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
            Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);

            // Ändra andra egenskaper
            textEffectFormat.Text = "Updated Text";
            textEffectFormat.FontBold = true;
            textEffectFormat.FontSize = 24;

            // Spara arbetsboken
            workbook.Save("TextEffectFormatDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


