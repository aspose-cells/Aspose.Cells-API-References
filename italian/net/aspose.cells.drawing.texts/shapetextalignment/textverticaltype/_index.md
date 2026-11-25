---
title: "ShapeTextAlignment.TextVerticalType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Ottiene e imposta la direzione del testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/textverticaltype/
---
## ShapeTextAlignment.TextVerticalType property

Ottiene e imposta la direzione del testo.

```csharp
public TextVerticalType TextVerticalType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma casella di testo con i parametri corretti
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Ottieni l'allineamento del testo e imposta il tipo di testo verticale
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Salva la cartella di lavoro
            workbook.Save("TextVerticalTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextVerticalType](../../textverticaltype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


