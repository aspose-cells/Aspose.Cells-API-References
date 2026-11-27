---
title: "TextEffectFormat.FontSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextEffectFormat-egenskap. Storleken i punkter för teckensnittet som används i WordArt"
type: docs
url: /sv/net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

Storleken (i punkter) på teckensnittet som används i WordArt.

```csharp
public int FontSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
            
            // Ange text och format
            textBox.Text = "Sample Text Effect";
            
            // Hämta texteffektformatet
            Shape shape = textBox;
            TextEffectFormat effectFormat = shape.TextEffect;
            
            // Ange teckensnittsegenskaper inklusive FontSize
            effectFormat.FontName = "Arial";
            effectFormat.FontBold = true;
            effectFormat.FontItalic = false;
            effectFormat.FontSize = 18; // Demonstrating FontSize property
            
            // Spara arbetsboken
            workbook.Save("TextEffectFontSizeDemo.xlsx");
            
            Console.WriteLine("Text effect with font size 18 created successfully.");
        }
    }
}
```

### Se även

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


