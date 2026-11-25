---
title: "ShapeTextAlignment.IsAutoMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Indica se il margine del riquadro di testo è automatico"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/isautomargin/
---
## ShapeTextAlignment.IsAutoMargin property

Indica se il margine del riquadro di testo è automatico.

```csharp
public bool IsAutoMargin { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsAutoMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Accedi all'allineamento del testo e imposta IsAutoMargin
            shape.TextBody.TextAlignment.IsAutoMargin = true;

            // Imposta del testo di esempio
            shape.Text = "Sample text with auto margins";

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextAlignmentIsAutoMarginDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


