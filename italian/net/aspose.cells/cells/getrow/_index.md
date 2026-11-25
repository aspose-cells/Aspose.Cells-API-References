---
title: "Cells.GetRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'elemento Row all'indice di riga della cella specificato"
type: docs
url: /it/net/aspose.cells/cells/getrow/
---
## Cells.GetRow method

Ottiene l'elemento [`Row`](../../row/) all'indice di riga della cella specificato.

```csharp
[Obsolete("Use Cells.CheckRow(int row) instead.")]
public Row GetRow(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga |

### Valore di ritorno

Se l'oggetto riga esiste, restituisce l'oggetto Row, altrimenti restituisce null.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.CheckRow(int row). Questo metodo sarà rimosso 12 mesi dopo, a partire da febbraio 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea celle nella riga 5 per garantire che la riga esista
            worksheet.Cells["A5"].PutValue("Row 5 Data");
            worksheet.Cells["B5"].PutValue(12345);

            try
            {
                // Chiama il metodo GetRow con parametro Int32
                Row resultRow = worksheet.Cells.GetRow(5);

                if (resultRow != null)
                {
                    // Dimostra la manipolazione delle righe
                    resultRow.Height = 20;
                    Console.WriteLine($"Retrieved row 5 successfully. Current height: {resultRow.Height} points");
                    
                    // Conta le celle nella riga
                    int cellCount = 0;
                    foreach (Cell cell in resultRow)
                    {
                        cellCount++;
                    }
                    Console.WriteLine($"Row 5 contains {cellCount} cells");
                }
                else
                {
                    Console.WriteLine("Row 5 not found in worksheet");
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid row index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRow: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("CellsMethodGetRowWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


