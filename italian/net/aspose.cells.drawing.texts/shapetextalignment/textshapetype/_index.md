---
title: "ShapeTextAlignment.TextShapeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Ottiene e imposta il tipo di trasformazione del testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/textshapetype/
---
## ShapeTextAlignment.TextShapeType property

Ottiene e imposta il tipo di trasformazione del testo.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di testo
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);

            // Ottieni l'allineamento del testo della forma
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Imposta la proprietà TextShapeType
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;

            // Salva la cartella di lavoro
            workbook.Save("TextShapeTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


