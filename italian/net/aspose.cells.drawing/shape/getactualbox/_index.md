---
title: "Shape.GetActualBox"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Ottieni la posizione e le dimensioni effettive della forma dopo aver applicato rotazione, capovolgimento, ecc."
type: docs
url: /it/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

Ottieni la posizione e le dimensioni effettive della forma (dopo aver applicato rotazione, capovolgimento, ecc.)

```csharp
public float[] GetActualBox()
```

### Valore di ritorno

Restituisce la posizione e le dimensioni nell'ordine x, y, w, h

### Osservazioni

Nota: l'interfaccia non è completamente funzionale, soprattutto le informazioni sulla posizione non sono corrette. Si consiglia di non utilizzare questa interfaccia finché la funzione non è completa.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // Ottieni le dimensioni reali della casella della forma
            float[] box = rectangle.GetActualBox();

            // Restituisci le dimensioni della casella
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // Salva la cartella di lavoro
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


