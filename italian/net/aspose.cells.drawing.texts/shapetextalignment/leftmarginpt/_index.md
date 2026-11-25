---
title: "ShapeTextAlignment.LeftMarginPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Restituisce il margine sinistro in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/
---
## ShapeTextAlignment.LeftMarginPt property

Restituisce il margine sinistro in unità di punti

```csharp
public double LeftMarginPt { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyLeftMarginPtDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            
            // Imposta il testo per la forma
            shape.Text = "Sample text with left margin";

            // Accedi all'allineamento del testo e imposta il margine sinistro in punti
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.LeftMarginPt = 2.0d;

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextAlignmentLeftMarginPtDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


