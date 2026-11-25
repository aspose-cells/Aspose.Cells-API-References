---
title: "TextEffectFormat.FontBold"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextEffectFormat. Indica se il carattere è in grassetto"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/fontbold/
---
## TextEffectFormat.FontBold property

Indica se il carattere è in grassetto.

```csharp
public bool FontBold { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di testo (restituisce direttamente l'oggetto TextBox)
            TextBox textbox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            textbox.Text = "Sample Text";

            // Ottieni il formato dell'effetto di testo
            TextEffectFormat effFormat = textbox.TextEffect;

            // Imposta le proprietà del carattere includendo il grassetto
            effFormat.FontName = "Arial";
            effFormat.FontBold = true;
            effFormat.FontItalic = false;
            effFormat.FontSize = 14;

            // Salva la cartella di lavoro
            workbook.Save("TextEffectFormatFontBoldDemo.xlsx");

            Console.WriteLine("Text effect format with bold font applied successfully.");
        }
    }
}
```

### Vedi anche

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


