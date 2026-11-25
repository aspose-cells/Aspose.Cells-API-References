---
title: "TextEffectFormat.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextEffectFormat. Il testo nel WordArt"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/text/
---
## TextEffectFormat.Text property

Il testo nel WordArt.

```csharp
public string Text { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi una forma di effetto di testo e imposta il suo testo
            Shape shape = sheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 14, false, false, 0, 0, 0, 0, 100, 100);

            // Accedi e modifica la proprietà testo dell'effetto di testo
            shape.TextEffect.Text = "Updated Text";

            // Verifica che il testo sia stato aggiornato
            Console.WriteLine("Text Effect Content: " + shape.TextEffect.Text);
        }
    }
}
```

### Vedi anche

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


