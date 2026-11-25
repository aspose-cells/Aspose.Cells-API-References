---
title: "Shape.AlternativeText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Restituisce o imposta la stringa di testo alternativo descrittiva dell'oggetto Shape"
type: docs
url: /it/net/aspose.cells.drawing/shape/alternativetext/
---
## Shape.AlternativeText property

Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [`Shape`](../).

```csharp
public string AlternativeText { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Imposta il testo alternativo per la forma
            shape.AlternativeText = "A rectangle shape with width 100 and height 200";

            // Salva la cartella di lavoro
            workbook.Save("ShapeAlternativeTextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


