---
title: "TextEffectFormat.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextEffectFormat-egenskap. Texten i WordArt"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/text/
---
## TextEffectFormat.Text property

Texten i WordArt.

```csharp
public string Text { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en texteffektsform och ange dess text
            Shape shape = sheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 14, false, false, 0, 0, 0, 0, 100, 100);

            // Åtkomst och ändring av texteffektens text-egenskap
            shape.TextEffect.Text = "Updated Text";

            // Verifiera att texten uppdaterades
            Console.WriteLine("Text Effect Content: " + shape.TextEffect.Text);
        }
    }
}
```

### Se även

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


