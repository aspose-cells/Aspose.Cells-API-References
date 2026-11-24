---
title: "TextEffectFormat.FontName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextEffectFormat-Eigenschaft. Der Name der im WordArt verwendeten Schrift"
type: docs
url: /de/net/aspose.cells.drawing/texteffectformat/fontname/
---
## TextEffectFormat.FontName property

Der Name der im WordArt verwendeten Schrift.

```csharp
public string FontName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine WordArt-Form hinzu
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Setze und erhalte die FontName-Eigenschaft
            shape.TextEffect.FontName = "+mn-ea";
            string fontName = shape.TextEffect.FontName;

            // Gib das Ergebnis aus
            Console.WriteLine("Font Name: " + fontName);
        }
    }
}
```

### Siehe auch

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


