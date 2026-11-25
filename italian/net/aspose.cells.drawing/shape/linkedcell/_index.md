---
title: "Shape.LinkedCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene o imposta l'intervallo del foglio di lavoro collegato al valore del controllo"
type: docs
url: /it/net/aspose.cells.drawing/shape/linkedcell/
---
## Shape.LinkedCell property

Ottiene o imposta l'intervallo del foglio di lavoro collegato al valore del controllo.

```csharp
public string LinkedCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Imposta la proprietà LinkedCell su B6
            shape.LinkedCell = "$B$6";

            // Cambia LinkedCell in A1 se era B6
            if (shape.LinkedCell.Equals("$B$6"))
            {
                shape.LinkedCell = "A1";
            }

            // Restituisci il valore corrente di LinkedCell
            Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


