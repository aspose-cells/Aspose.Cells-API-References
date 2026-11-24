---
title: "TextEffectFormat.SetTextEffect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextEffectFormat-Methode. Legt den vordefinierten Texteffekt fest"
type: docs
url: /de/net/aspose.cells.drawing/texteffectformat/settexteffect/
---
## TextEffectFormat.SetTextEffect method

Legt den voreingestellten Texteffekt fest.

```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Effekt | MsoPresetTextEffect | Der voreingestellte Texteffekt. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form für WordArt hinzu
            Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);

            // Erhalte das TextEffectFormat der Form
            TextEffectFormat textEffectFormat = wordArt.TextEffect;

            try
            {
                // Rufe die SetTextEffect-Methode mit dem MsoPresetTextEffect-Parameter auf
                textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);

                // Setze zusätzliche Eigenschaften für das WordArt
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = false;
                textEffectFormat.FontSize = 24;

                Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


