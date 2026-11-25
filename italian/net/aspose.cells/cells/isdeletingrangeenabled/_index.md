---
title: "Cells.IsDeletingRangeEnabled"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Verifica se l'intervallo può essere eliminato"
type: docs
url: /it/net/aspose.cells/cells/isdeletingrangeenabled/
---
## Cells.IsDeletingRangeEnabled method

Verifica se l'intervallo può essere eliminato.

```csharp
public bool IsDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | L'indice della riga iniziale dell'intervallo. |
| startColumn | Int32 | L'indice della colonna iniziale dell'intervallo. |
| totalRows | Int32 | Il numero di righe nell'intervallo. |
| totalColumns | Int32 | Il numero di colonne nell'intervallo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodIsDeletingRangeEnabledWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola dati di esempio nelle celle A1:C5
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row, col].Value = $"Data{row}_{col}";
                }
            }

            try
            {
                // Verifica se l'eliminazione di 5 righe x 3 colonne a partire da A1 è abilitata
                bool canDelete = cells.IsDeletingRangeEnabled(0, 0, 5, 3);
                Console.WriteLine($"Can delete range: {canDelete}");

                if (canDelete)
                {
                    // Elimina l'intervallo A1:C5 e sposta le celle verso l'alto
                    cells.DeleteRange(0, 0, 4, 2, ShiftType.Up);
                    Console.WriteLine("Deleted range A1:C5 successfully");
                }

                workbook.Save("IsDeletingRangeEnabledOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during range deletion: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


