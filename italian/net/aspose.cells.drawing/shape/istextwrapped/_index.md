---
title: "Shape.IsTextWrapped"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il tipo di avvolgimento del testo della forma che contiene testo"
type: docs
url: /it/net/aspose.cells.drawing/shape/istextwrapped/
---
## Shape.IsTextWrapped property

Ottiene e imposta il tipo di interruzione del testo della forma che contiene testo.

```csharp
public bool IsTextWrapped { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma e imposta del testo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "This is a sample text that will demonstrate text wrapping functionality";

            // Dimostra la proprietà IsTextWrapped
            Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
            
            // Attiva/disattiva l'avvolgimento del testo
            shape.IsTextWrapped = !shape.IsTextWrapped;
            Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


