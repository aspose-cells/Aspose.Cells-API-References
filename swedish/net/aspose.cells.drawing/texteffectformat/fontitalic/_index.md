---
title: "TextEffectFormat.FontItalic"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextEffectFormat-egenskap. Anger om teckensnittet är kursivt"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/fontitalic/
---
## TextEffectFormat.FontItalic property

Anger om teckensnittet är kursiv.

```csharp
public bool FontItalic { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med texteffekt
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Hämta texteffektformatet
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Ställ in FontItalic till true
            textEffectFormat.FontItalic = true;
            Console.WriteLine("FontItalic after setting to true: " + textEffectFormat.FontItalic);

            // Ställ in FontItalic till false
            textEffectFormat.FontItalic = false;
            Console.WriteLine("FontItalic after setting to false: " + textEffectFormat.FontItalic);

            // Spara arbetsboken
            workbook.Save("TextEffectFormatFontItalicDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


