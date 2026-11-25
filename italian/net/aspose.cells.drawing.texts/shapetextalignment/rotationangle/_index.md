---
title: "ShapeTextAlignment.RotationAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Ottiene e imposta la rotazione della forma"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/rotationangle/
---
## ShapeTextAlignment.RotationAngle property

Ottiene e imposta la rotazione della shape.

```csharp
public double RotationAngle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 200, 300, 400);
            
            // Imposta il testo della forma
            shape.Text = "Rotated Text";
            
            // Accedi all'allineamento del testo e imposta l'angolo di rotazione
            shape.TextBody.TextAlignment.RotationAngle = 90;

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextRotationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


