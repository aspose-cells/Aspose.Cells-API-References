---
title: "WorksheetCollection.CreateRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection metodo. Crea un oggetto Range da un indirizzo dell'intervallo"
type: docs
url: /it/net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Crea un oggetto [`Range`](../../range/) da un indirizzo dell'intervallo.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| address | String | L'indirizzo dell'intervallo. |
| sheetIndex | Int32 | L'indice del foglio. |

### Valore di ritorno

Un oggetto [`Range`](../../range/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 6; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Crea un intervallo usando l'indirizzo stringa e l'indice del foglio
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);

            // Dimostra l'uso dell'intervallo
            Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
            Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
            Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


