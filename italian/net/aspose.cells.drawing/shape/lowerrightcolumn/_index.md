---
title: "Shape.LowerRightColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta l'indice della colonna dell'angolo in basso a destra"
type: docs
url: /it/net/aspose.cells.drawing/shape/lowerrightcolumn/
---
## Shape.LowerRightColumn property

Rappresenta l'indice della colonna dell'angolo in basso a destra.

```csharp
public int LowerRightColumn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Imposta e visualizza il valore iniziale di LowerRightColumn
            shape.LowerRightColumn = 3;
            Console.WriteLine("Initial LowerRightColumn: " + shape.LowerRightColumn);

            // Modifica LowerRightColumn se è uguale a 3
            if (shape.LowerRightColumn == 3)
            {
                shape.LowerRightColumn = 1;
                Console.WriteLine("Modified LowerRightColumn: " + shape.LowerRightColumn);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


