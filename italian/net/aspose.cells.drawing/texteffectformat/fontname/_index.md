---
title: "TextEffectFormat.FontName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextEffectFormat. Il nome del carattere usato nel WordArt"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/fontname/
---
## TextEffectFormat.FontName property

Il nome del carattere utilizzato nel WordArt.

```csharp
public string FontName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma WordArt
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Imposta e ottieni la proprietà FontName
            shape.TextEffect.FontName = "+mn-ea";
            string fontName = shape.TextEffect.FontName;

            // Restituisci il risultato
            Console.WriteLine("Font Name: " + fontName);
        }
    }
}
```

### Vedi anche

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


