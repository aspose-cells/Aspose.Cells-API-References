---
title: "TextEffectFormat.PresetShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextEffectFormat. Ottiene e imposta il tipo di forma predefinita"
type: docs
url: /it/net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

Ottiene e imposta il tipo di forma predefinito.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyPresetShapeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con effetto di testo
            Shape shape = worksheet.Shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect1,
                "Sample Text",
                "Arial",
                18,
                false,
                false,
                0,
                0,
                100,
                200,
                0,
                0);

            // Ottieni il formato dell'effetto di testo
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Imposta e ottieni la proprietà PresetShape
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
            Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);

            // Modifica altre proprietà
            textEffectFormat.Text = "Updated Text";
            textEffectFormat.FontBold = true;
            textEffectFormat.FontSize = 24;

            // Salva la cartella di lavoro
            workbook.Save("TextEffectFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


