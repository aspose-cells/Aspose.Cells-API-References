---
title: "Shape.Title"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Specifica la didascalia del titolo dell'oggetto forma corrente"
type: docs
url: /it/net/aspose.cells.drawing/shape/title/
---
## Shape.Title property

Specifica il titolo (didascalia) dell'oggetto shape corrente.

```csharp
public string Title { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Imposta il titolo della forma
            shape.Title = "title1";

            // Verifica che il titolo sia stato impostato
            Console.WriteLine("Shape title: " + shape.Title);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


