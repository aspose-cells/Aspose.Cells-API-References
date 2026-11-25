---
title: "TextEffectFormat.RotatedChars"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextEffectFormat. Se true i caratteri nel WordArt specificato sono ruotati di 90 gradi rispetto alla forma di delimitazione del WordArt"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

Se vero, i caratteri nel WordArt specificato sono ruotati di 90 gradi rispetto alla forma di delimitazione del WordArt.

```csharp
public bool RotatedChars { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con effetto di testo
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 100, 100, 200, 50);

            // Ottieni il formato dell'effetto di testo
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Imposta la proprietà RotatedChars su true
            textEffectFormat.RotatedChars = true;

            // Salva la cartella di lavoro
            workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");

            // Verifica la proprietà RotatedChars
            Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
        }
    }
}
```

### Vedi anche

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


