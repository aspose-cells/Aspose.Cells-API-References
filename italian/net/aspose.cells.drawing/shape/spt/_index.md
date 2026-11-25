---
title: "Shape.Spt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Specifica un numero opzionale che un'applicazione può utilizzare per associare la forma particolare a un tipo di forma definito."
type: docs
url: /it/net/aspose.cells.drawing/shape/spt/
---
## Shape.Spt property

Specifica un numero opzionale che un'applicazione può utilizzare per associare la forma specifica a un tipo di forma definito.

```csharp
public int Spt { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySptDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);

            // Ottieni e visualizza la proprietà Spt.
            int spt = shape.Spt;
            Console.WriteLine("Shape Spt value: " + spt);

            // Crea una nuova forma ovale per dimostrare un valore Spt diverso.
            Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
            Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


