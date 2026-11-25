---
title: "Cells.MoveRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Sposta l'intervallo"
type: docs
url: /it/net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Sposta l'intervallo.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceArea | CellArea | L'intervallo che dovrebbe essere spostato. |
| destRow | Int32 | La riga di destinazione. |
| destColumn | Int32 | La colonna di destinazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Inserisci valori nelle celle
            cells["A1"].PutValue("Original");
            cells["B1"].PutValue(100);
            cells["A2"].PutValue("Data");
            cells["B2"].PutValue(200);

            // Definisci l'area di celle da spostare (A1:B2)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            // Sposta l'intervallo verso il basso di 2 righe e verso destra di 3 colonne
            cells.MoveRange(area, 2, 3);

            // Salva la cartella di lavoro
            workbook.Save("MoveRangeExample.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


