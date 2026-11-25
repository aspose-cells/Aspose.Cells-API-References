---
title: "Cells.ExportTypeArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Esporta il tipo di valore della cella nella raccolta Cells in un oggetto array bidimensionale"
type: docs
url: /it/net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

Esporta il tipo di valore della cella nella raccolta [`Cells`](../) in un oggetto array bidimensionale.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Il numero di riga della prima cella da esportare. |
| firstColumn | Int32 | Il numero di colonna della prima cella da esportare. |
| totalRows | Int32 | Numero di righe da esportare. |
| totalColumns | Int32 | Numero di colonne da esportare. |

### Valore di ritorno

Oggetto array esportato che rappresenta i tipi di valore delle celle.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta valori nelle celle
            cells["A1"].PutValue(10);
            cells["B1"].PutValue("Hello");
            cells["A2"].PutValue(true);
            cells["B2"].PutValue(DateTime.Now);

            // Esporta i tipi di cella in un array 2D
            CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);

            // Visualizza i risultati
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 2; j++)
                {
                    Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
                }
            }

            // Dimostrare il caso di eccezione
            try
            {
                CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Exception caught as expected: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


