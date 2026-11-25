---
title: "Shape.Geometry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene la geometria."
type: docs
url: /it/net/aspose.cells.drawing/shape/geometry/
---
## Shape.Geometry property

Ottiene la geometria

```csharp
public Geometry Geometry { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGeometryDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Verifica le proprietà della geometria.
            if (shape.Geometry != null)
            {
                Console.WriteLine("Shape has geometry path with " + shape.Geometry.ShapeAdjustValues.Count + " adjustment points");
                
                // Aggiungi un punto di regolazione (dimostrazione della modifica della geometria).
                shape.Geometry.ShapeAdjustValues.Add("adj1", 0.5);
                Console.WriteLine("Added adjustment point. Total now: " + shape.Geometry.ShapeAdjustValues.Count);
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeGeometryDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Geometry](../../geometry/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


