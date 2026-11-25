---
title: "Shape.HeightScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta la scala dell'altezza in unità di percentuale dell'altezza originale dell'immagine. Se la forma non è un'immagine, la proprietà HeightScale restituisce solo 100"
type: docs
url: /it/net/aspose.cells.drawing/shape/heightscale/
---
## Shape.HeightScale property

Ottiene e imposta la scala dell'altezza, in unità di percentuale dell'altezza originale dell'immagine. Se la forma non è un'immagine, la proprietà HeightScale restituisce solo 100;

```csharp
public int HeightScale { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);

            // Imposta la scala di altezza iniziale
            shape.HeightScale = 50;
            Console.WriteLine("Initial HeightScale: " + shape.HeightScale);

            // Modifica la scala di altezza se la condizione è soddisfatta
            if (shape.HeightScale == 50)
            {
                shape.HeightScale = 75;
                Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


