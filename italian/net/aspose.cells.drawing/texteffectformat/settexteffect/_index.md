---
title: "TextEffectFormat.SetTextEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TextEffectFormat. Imposta l'effetto di testo predefinito"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/settexteffect/
---
## TextEffectFormat.SetTextEffect method

Imposta l'effetto di testo predefinito.

```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| effetto | MsoPresetTextEffect | L'effetto di testo predefinito. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per WordArt
            Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);

            // Ottieni il TextEffectFormat della forma
            TextEffectFormat textEffectFormat = wordArt.TextEffect;

            try
            {
                // Chiama il metodo SetTextEffect con il parametro MsoPresetTextEffect
                textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);

                // Imposta proprietà aggiuntive per il WordArt
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = false;
                textEffectFormat.FontSize = 24;

                Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


