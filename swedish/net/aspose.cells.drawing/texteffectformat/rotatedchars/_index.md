---
title: "TextEffectFormat.RotatedChars"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextEffectFormat-egenskap. Om true roteras tecken i den angivna WordArt 90 grader relativt WordArts omgivande form"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

Om sant roteras tecknen i den angivna WordArt med 90 grader i förhållande till WordArts omgivande form.

```csharp
public bool RotatedChars { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med texteffekt
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 100, 100, 200, 50);

            // Hämta texteffektformatet
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Ställ in RotatedChars-egenskapen till true
            textEffectFormat.RotatedChars = true;

            // Spara arbetsboken
            workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");

            // Verifiera RotatedChars-egenskapen
            Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
        }
    }
}
```

### Se även

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


