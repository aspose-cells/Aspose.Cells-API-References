---
title: "Shape.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il testo di questa forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/text/
---
## Shape.Text property

Ottiene e imposta il testo di questa forma.

```csharp
public string Text { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Imposta il testo se nullo
            if (shape.Text == null)
            {
                shape.Text = "This is a test.";
            }

            // Modifica il testo
            shape.Text = "Updated text demo";

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


