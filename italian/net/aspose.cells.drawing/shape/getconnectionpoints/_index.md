---
title: "Shape.GetConnectionPoints"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Ottieni i punti di connessione"
type: docs
url: /it/net/aspose.cells.drawing/shape/getconnectionpoints/
---
## Shape.GetConnectionPoints method

Ottieni i punti di connessione

```csharp
public float[][] GetConnectionPoints()
```

### Valore di ritorno

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetConnectionPointsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Ottieni i punti di connessione della forma
            float[][] points = shape.GetConnectionPoints();

            // Stampa i punti di connessione
            Console.WriteLine("Connection Points:");
            for (int i = 0; i < points.Length; i++)
            {
                Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


