---
title: "Classe TextEffectFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.TextEffectFormat. Contiene proprietà e metodi che si applicano agli oggetti WordArt"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/
---
## TextEffectFormat class

Contiene proprietà e metodi che si applicano agli oggetti WordArt.

```csharp
public class TextEffectFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | Indica se il carattere è in grassetto. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | Indica se il carattere è in corsivo. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | Il nome del carattere utilizzato nel WordArt. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | La dimensione (in punti) del carattere utilizzato nel WordArt. |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | Ottiene e imposta il tipo di forma predefinito. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | Se vero, i caratteri nel WordArt specificato sono ruotati di 90 gradi rispetto alla forma di delimitazione del WordArt. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | Il testo nel WordArt. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | Imposta l'effetto di testo predefinito. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextEffectFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            
            // Aggiungi forma di effetto testo
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            
            // Modifica l'effetto di testo
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;
            textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
            
            // Salva la cartella di lavoro
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


