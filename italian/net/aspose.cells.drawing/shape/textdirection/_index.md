---
title: "Shape.TextDirection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene/Imposta la direzione del flusso di testo per questo oggetto"
type: docs
url: /it/net/aspose.cells.drawing/shape/textdirection/
---
## Shape.TextDirection property

Ottiene/Imposta la direzione del flusso di testo per questo oggetto.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di testo
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample Text";

            // Imposta e dimostra la proprietà TextDirection
            shape.TextDirection = TextDirectionType.Context;
            Console.WriteLine("Initial TextDirection: " + shape.TextDirection);

            // Cambia la direzione del testo
            shape.TextDirection = TextDirectionType.LeftToRight;
            Console.WriteLine("Updated TextDirection: " + shape.TextDirection);

            // Salva la cartella di lavoro
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


