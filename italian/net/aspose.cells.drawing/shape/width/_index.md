---
title: "Shape.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta la larghezza della forma in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/width/
---
## Shape.Width property

Rappresenta la larghezza della shape, in unità di pixel.

```csharp
public int Width { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 50);

            // Imposta la larghezza iniziale e visualizzala
            shape.Width = 300;
            Console.WriteLine("Initial width: " + shape.Width);

            // Modifica la larghezza in base a una condizione
            if (shape.Width == 300)
                shape.Width = 150;

            Console.WriteLine("Modified width: " + shape.Width);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


