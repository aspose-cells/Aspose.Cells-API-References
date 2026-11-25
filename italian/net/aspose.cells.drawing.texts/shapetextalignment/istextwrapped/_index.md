---
title: "ShapeTextAlignment.IsTextWrapped"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Ottiene o imposta il tipo di avvolgimento del testo della forma che contiene testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/istextwrapped/
---
## ShapeTextAlignment.IsTextWrapped property

Ottiene o imposta il tipo di avvolgimento del testo della forma che contiene il testo.

```csharp
public bool IsTextWrapped { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Imposta il testo della forma
            shape.Text = "This is a long text that should be wrapped when IsTextWrapped is set to true";

            // Ottieni l'allineamento del testo e imposta IsTextWrapped
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.IsTextWrapped = true;

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


