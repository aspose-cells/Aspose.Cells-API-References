---
title: "Shape.WidthScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta la scala di larghezza in unità di percentuale della larghezza originale dell'immagine. Se la forma non è un'immagine, la proprietà WidthScale restituisce solo 100"
type: docs
url: /it/net/aspose.cells.drawing/shape/widthscale/
---
## Shape.WidthScale property

Ottiene e imposta la scala di larghezza, in unità di percentuale della larghezza originale dell'immagine. Se la forma non è un'immagine, la proprietà WidthScale restituisce solo 100;

```csharp
public int WidthScale { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Imposta la scala di larghezza iniziale
            shape.WidthScale = 50;
            Console.WriteLine("Initial WidthScale: " + shape.WidthScale);

            // Modifica la scala di larghezza se la condizione è soddisfatta
            if (shape.WidthScale == 50)
            {
                shape.WidthScale = 75;
                Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeWidthScaleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


