---
title: "TextEffectFormat.FontSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextEffectFormat-Eigenschaft. Die Größe in Punkten der im WordArt verwendeten Schrift"
type: docs
url: /de/net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

Die Größe (in Punkten) der im WordArt verwendeten Schrift.

```csharp
public int FontSize { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
            
            // Text und Format festlegen
            textBox.Text = "Sample Text Effect";
            
            // Erhalte das TextEffectFormat
            Shape shape = textBox;
            TextEffectFormat effectFormat = shape.TextEffect;
            
            // Setze Schriftarteigenschaften einschließlich FontSize
            effectFormat.FontName = "Arial";
            effectFormat.FontBold = true;
            effectFormat.FontItalic = false;
            effectFormat.FontSize = 18; // Demonstrating FontSize property
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextEffectFontSizeDemo.xlsx");
            
            Console.WriteLine("Text effect with font size 18 created successfully.");
        }
    }
}
```

### Siehe auch

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


