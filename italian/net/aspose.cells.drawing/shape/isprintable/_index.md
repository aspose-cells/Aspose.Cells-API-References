---
title: "Shape.IsPrintable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se l'oggetto è stampabile. Se False questa forma non verrà stampata durante la stampa"
type: docs
url: /it/net/aspose.cells.drawing/shape/isprintable/
---
## Shape.IsPrintable property

Indica se l'oggetto è stampabile. Se False, questa forma non verrà stampata durante la stampa.

```csharp
public bool IsPrintable { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsPrintableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Dimostrare la proprietà IsPrintable
            Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);

            // Attiva/disattiva la proprietà IsPrintable
            shape.IsPrintable = !shape.IsPrintable;
            Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);

            // Imposta esplicitamente IsPrintable a false
            shape.IsPrintable = false;
            Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


