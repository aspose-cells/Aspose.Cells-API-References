---
title: "ShapeTextAlignment.TextHorizontalOverflow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Ottiene e imposta il tipo di overflow orizzontale del testo nella casella di testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/
---
## ShapeTextAlignment.TextHorizontalOverflow property

Ottiene e imposta il tipo di overflow orizzontale del testo nella casella di testo.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di testo
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 50);
            textBox.Text = "This is a long text that demonstrates horizontal overflow behavior";

            // Imposta l'overflow orizzontale su Clip
            textBox.TextBody.TextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;

            // Salva la cartella di lavoro
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


