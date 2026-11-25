---
title: "Shape.MoveToRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Sposta la forma in un intervallo specificato"
type: docs
url: /it/net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

Sposta la forma a un intervallo specificato.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| bottomRow | Int32 | Indice della riga in basso a destra |
| rightColumn | Int32 | Indice della colonna in basso a destra |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodMoveToRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Sposta la forma in un intervallo specifico
            shape.MoveToRange(12, 3, 13, 5);

            // Salva la cartella di lavoro
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


