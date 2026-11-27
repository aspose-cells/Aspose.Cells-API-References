---
title: "TextEffectFormat.SetTextEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextEffectFormat-metod. Anger den förinställda texteffekten"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/settexteffect/
---
## TextEffectFormat.SetTextEffect method

Anger den förinställda texteffekten.

```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| effekt | MsoPresetTextEffect | Den förinställda texteffekten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för WordArt
            Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);

            // Hämta TextEffectFormat för formen
            TextEffectFormat textEffectFormat = wordArt.TextEffect;

            try
            {
                // Anropa SetTextEffect-metoden med MsoPresetTextEffect-parameter
                textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);

                // Ställ in ytterligare egenskaper för WordArt
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = false;
                textEffectFormat.FontSize = 24;

                Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


