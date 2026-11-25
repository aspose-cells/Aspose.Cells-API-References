---
title: "TextEffectFormat.FontItalic"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextEffectFormat. Indica se il carattere è in corsivo"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/fontitalic/
---
## TextEffectFormat.FontItalic property

Indica se il carattere è in corsivo.

```csharp
public bool FontItalic { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontItalicDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con effetto di testo
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Ottieni il formato dell'effetto di testo
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Imposta FontItalic su true
            textEffectFormat.FontItalic = true;
            Console.WriteLine("FontItalic after setting to true: " + textEffectFormat.FontItalic);

            // Imposta FontItalic su false
            textEffectFormat.FontItalic = false;
            Console.WriteLine("FontItalic after setting to false: " + textEffectFormat.FontItalic);

            // Salva la cartella di lavoro
            workbook.Save("TextEffectFormatFontItalicDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


