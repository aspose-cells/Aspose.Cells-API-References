---
title: "TextEffectFormat.RotatedChars"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextEffectFormat-Eigenschaft. Wenn true, werden die Zeichen im angegebenen WordArt um 90 Grad relativ zur Begrenzungsform des WordArt gedreht"
type: docs
url: /de/net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

Wenn true, werden die Zeichen im angegebenen WordArt um 90 Grad relativ zur Begrenzungsform des WordArt gedreht.

```csharp
public bool RotatedChars { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyRotatedCharsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form mit Texteffekt hinzu
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 100, 100, 200, 50);

            // Erhalte das TextEffectFormat
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Setze RotatedChars-Eigenschaft auf true
            textEffectFormat.RotatedChars = true;

            // Speichere die Arbeitsmappe
            workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");

            // Verifiziere die RotatedChars-Eigenschaft
            Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
        }
    }
}
```

### Siehe auch

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


