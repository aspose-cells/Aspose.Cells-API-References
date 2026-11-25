---
title: "CellsHelper.ColumnIndexToName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Ottiene il nome della colonna in base all'indice della colonna"
type: docs
url: /it/net/aspose.cells/cellshelper/columnindextoname/
---
## CellsHelper.ColumnIndexToName method

Ottiene il nome della colonna in base all'indice della colonna.

```csharp
public static string ColumnIndexToName(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |

### Valore di ritorno

Nome della colonna.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta valori nelle celle per dimostrare la conversione da indice di colonna a nome
            worksheet.Cells["A1"].PutValue("Column Index");
            worksheet.Cells["B1"].PutValue("Column Name");

            // Dimostra ColumnIndexToName per gli indici 0-4
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i);
                string columnName = CellsHelper.ColumnIndexToName(i);
                worksheet.Cells[i + 1, 1].PutValue(columnName);
            }

            // Salva la cartella di lavoro
            workbook.Save("ColumnIndexToNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


