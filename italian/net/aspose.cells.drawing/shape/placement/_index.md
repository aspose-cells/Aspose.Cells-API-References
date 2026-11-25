---
title: "Shape.Placement"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro."
type: docs
url: /it/net/aspose.cells.drawing/shape/placement/
---
## Shape.Placement property

Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro.

```csharp
public PlacementType Placement { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPlacementDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);

            // Dimostra la proprietà Placement
            Console.WriteLine("Original Placement: " + shape.Placement);
            
            // Modifica il tipo di posizionamento.
            shape.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Modified Placement: " + shape.Placement);

            // Salva la cartella di lavoro
            workbook.Save("ShapePlacementDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


