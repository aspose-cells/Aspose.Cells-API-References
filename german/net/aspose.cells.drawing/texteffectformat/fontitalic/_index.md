---
title: "TextEffectFormat.FontItalic"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextEffectFormat-Eigenschaft. Gibt an, ob die Schrift kursiv ist"
type: docs
url: /de/net/aspose.cells.drawing/texteffectformat/fontitalic/
---
## TextEffectFormat.FontItalic property

Gibt an, ob die Schrift kursiv ist.

```csharp
public bool FontItalic { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontItalicDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form mit Texteffekt hinzu
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Erhalte das TextEffectFormat
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Setze FontItalic auf true
            textEffectFormat.FontItalic = true;
            Console.WriteLine("FontItalic after setting to true: " + textEffectFormat.FontItalic);

            // Setze FontItalic auf false
            textEffectFormat.FontItalic = false;
            Console.WriteLine("FontItalic after setting to false: " + textEffectFormat.FontItalic);

            // Speichere die Arbeitsmappe
            workbook.Save("TextEffectFormatFontItalicDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


