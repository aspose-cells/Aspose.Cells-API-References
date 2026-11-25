---
title: "ShapeTextAlignment.TextVerticalOverflow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Ottiene e imposta il tipo di overflow verticale del testo nella casella di testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/
---
## ShapeTextAlignment.TextVerticalOverflow property

Ottiene e imposta il tipo di overflow verticale del testo nella casella di testo.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Imposta il testo che potrebbe traboccare verticalmente
            shape.Text = "This is a long text that might overflow vertically if not clipped properly";

            // Ottieni l'allineamento del testo e imposta l'overflow verticale su Clip
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;

            // Salva la cartella di lavoro
            workbook.Save("TextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


