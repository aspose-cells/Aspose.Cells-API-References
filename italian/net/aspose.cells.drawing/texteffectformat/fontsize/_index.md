---
title: "TextEffectFormat.FontSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextEffectFormat. La dimensione in punti del carattere usato nel WordArt"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

La dimensione (in punti) del carattere utilizzato nel WordArt.

```csharp
public int FontSize { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
            
            // Imposta testo e formato
            textBox.Text = "Sample Text Effect";
            
            // Ottieni il formato dell'effetto di testo
            Shape shape = textBox;
            TextEffectFormat effectFormat = shape.TextEffect;
            
            // Imposta le proprietà del carattere includendo FontSize
            effectFormat.FontName = "Arial";
            effectFormat.FontBold = true;
            effectFormat.FontItalic = false;
            effectFormat.FontSize = 18; // Demonstrating FontSize property
            
            // Salva la cartella di lavoro
            workbook.Save("TextEffectFontSizeDemo.xlsx");
            
            Console.WriteLine("Text effect with font size 18 created successfully.");
        }
    }
}
```

### Vedi anche

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


