---
title: "Shape.Bottom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/bottom/
---
## Shape.Bottom property

Rappresenta la larghezza dello spostamento verticale della shape dalla sua riga d'angolo inferiore, in unità di pixel.

```csharp
public int Bottom { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta la posizione iniziale
            shape.Top = 200;
            shape.Left = 200;

            // Dimostra la proprietà Bottom
            Console.WriteLine("Original Bottom position: " + shape.Bottom);

            // Modifica la posizione Bottom
            if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
            {
                shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
                Console.WriteLine("New Bottom position: " + shape.Bottom);
                Console.WriteLine("New Top position: " + shape.Top);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


