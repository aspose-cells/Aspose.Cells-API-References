---
title: "CellsHelper.CellIndexToName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Ottiene il nome della cella in base ai suoi indici di riga e colonna"
type: docs
url: /it/net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

Ottiene il nome della cella in base ai suoi indici di riga e colonna.

```csharp
public static string CellIndexToName(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |
| colonna | Int32 | Indice colonna. |

### Valore di ritorno

Nome della cella.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);

            // Ottieni il nome della cella da indici di riga e colonna
            string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)

            // Restituisci il risultato
            Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


