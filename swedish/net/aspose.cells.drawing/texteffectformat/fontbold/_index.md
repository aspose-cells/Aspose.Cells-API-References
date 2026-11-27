---
title: "TextEffectFormat.FontBold"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextEffectFormat-egenskap. Anger om teckensnittet är fetstil"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/fontbold/
---
## TextEffectFormat.FontBold property

Anger om teckensnittet är fetstil.

```csharp
public bool FontBold { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textrutaform (returnerar TextBox-objektet direkt)
            TextBox textbox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            textbox.Text = "Sample Text";

            // Hämta texteffektformatet
            TextEffectFormat effFormat = textbox.TextEffect;

            // Ange teckensnittsegenskaper inklusive fetstil
            effFormat.FontName = "Arial";
            effFormat.FontBold = true;
            effFormat.FontItalic = false;
            effFormat.FontSize = 14;

            // Spara arbetsboken
            workbook.Save("TextEffectFormatFontBoldDemo.xlsx");

            Console.WriteLine("Text effect format with bold font applied successfully.");
        }
    }
}
```

### Se även

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


