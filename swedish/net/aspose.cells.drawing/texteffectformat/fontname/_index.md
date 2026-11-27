---
title: "TextEffectFormat.FontName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextEffectFormat-egenskap. Namnet på teckensnittet som används i WordArt"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/fontname/
---
## TextEffectFormat.FontName property

Namnet på teckensnittet som används i WordArt.

```csharp
public string FontName { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en WordArt-form
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Ställ in och hämta FontName-egenskapen
            shape.TextEffect.FontName = "+mn-ea";
            string fontName = shape.TextEffect.FontName;

            // Skriv ut resultatet
            Console.WriteLine("Font Name: " + fontName);
        }
    }
}
```

### Se även

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


