---
title: "Shape.GetLinkedCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Ottiene l'intervallo collegato al valore del controllo"
type: docs
url: /it/net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

Ottiene l'intervallo collegato al valore del controllo.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Valore di ritorno

L'intervallo collegato al valore del controllo.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLinkedCellWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma e imposta la sua cella collegata
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.LinkedCell = "A1";

            // Ottieni l'indirizzo della cella collegata con diverse combinazioni di parametri
            string link1 = shape.GetLinkedCell(false, false); // Returns absolute reference like "$A$1"
            string link2 = shape.GetLinkedCell(true, false);   // Returns relative reference like "A1"
            string link3 = shape.GetLinkedCell(false, true);   // Returns R1C1 style absolute reference

            Console.WriteLine("Linked cell (absolute A1): " + link1);
            Console.WriteLine("Linked cell (relative A1): " + link2);
            Console.WriteLine("Linked cell (R1C1 style): " + link3);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


