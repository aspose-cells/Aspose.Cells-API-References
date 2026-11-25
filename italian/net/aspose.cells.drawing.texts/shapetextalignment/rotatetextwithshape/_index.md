---
title: "ShapeTextAlignment.RotateTextWithShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Indica se ruotare il testo con la forma"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/
---
## ShapeTextAlignment.RotateTextWithShape property

Indica se il testo è ruotato con la forma.

```csharp
public bool RotateTextWithShape { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma casella di testo con i parametri corretti
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Accedi alle proprietà di allineamento del testo
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            
            // Imposta la proprietà RotateTextWithShape
            textAlignment.RotateTextWithShape = true;

            // Ruota la forma per dimostrare l'effetto
            shape.RotationAngle = 45;

            // Salva la cartella di lavoro
            workbook.Save("RotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


