---
title: "ShapeTextAlignment.RightMarginPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Restituisce il margine destro in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/
---
## ShapeTextAlignment.RightMarginPt property

Restituisce il margine destro in unità di punti

```csharp
public double RightMarginPt { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Accedi all'allineamento del testo
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Imposta il margine destro in punti
            shapeTextAlignment.RightMarginPt = 2.0d;

            // Verifica la proprietà ottenendo nuovamente il valore
            Console.WriteLine("Right Margin in Points: " + shapeTextAlignment.RightMarginPt);
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


