---
title: "Cells.ExportArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Esporta i dati nella raccolta Cells in un oggetto array bidimensionale"
type: docs
url: /it/net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

Esporta i dati nella raccolta [`Cells`](../) in un oggetto array bidimensionale.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Il numero di riga della prima cella da esportare. |
| firstColumn | Int32 | Il numero di colonna della prima cella da esportare. |
| totalRows | Int32 | Numero di righe da esportare |
| totalColumns | Int32 | Numero di colonne da esportare |

### Valore di ritorno

Oggetto array dei valori di cella esportati.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola alcuni dati di esempio
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[1, 0].PutValue(10);
            cells[1, 1].PutValue(20);

            try
            {
                // Esporta i dati in un array
                object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
                
                // Visualizza l'array esportato
                for (int i = 0; i < 2; i++)
                {
                    for (int j = 0; j < 2; j++)
                    {
                        Console.Write(dataArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error exporting array: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


