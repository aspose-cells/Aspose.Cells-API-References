---
title: "Shape.Right"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta la larghezza dello spostamento orizzontale della forma dalla sua colonna d'angolo inferiore destro, in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/shape/right/
---
## Shape.Right property

Rappresenta la larghezza dello spostamento orizzontale della shape dalla sua colonna dell'angolo in basso a destra, in unità di pixel.

```csharp
public int Right { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Imposta e ottieni la proprietà Right
            shape.Right = 200;
            Console.WriteLine("Shape Right position: " + shape.Right);

            // Modifica la proprietà Right in modo condizionale
            if (shape.Right == 200)
                shape.Right = 150;

            Console.WriteLine("Modified Shape Right position: " + shape.Right);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


