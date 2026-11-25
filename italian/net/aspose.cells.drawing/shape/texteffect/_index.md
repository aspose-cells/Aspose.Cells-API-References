---
title: "Shape.TextEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Restituisce un oggetto TextEffectFormat che contiene le proprietà di formattazione dell'effetto testo per la forma specificata. Si applica agli oggetti Shape che rappresentano WordArt."
type: docs
url: /it/net/aspose.cells.drawing/shape/texteffect/
---
## Shape.TextEffect property

Restituisce un oggetto TextEffectFormat che contiene le proprietà di formattazione degli effetti di testo per la forma specificata. Si applica agli oggetti Shape che rappresentano WordArt.

```csharp
public TextEffectFormat TextEffect { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextEffectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma WordArt con i parametri corretti.
            Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);

            // Verifica se è WordArt e accedi alle proprietà TextEffect.
            if (shape.IsWordArt)
            {
                TextEffectFormat textEffectFormat = shape.TextEffect;
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = true;
                textEffectFormat.FontName = "Arial";
                textEffectFormat.FontSize = 14;
            }

            // Salva la cartella di lavoro
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


