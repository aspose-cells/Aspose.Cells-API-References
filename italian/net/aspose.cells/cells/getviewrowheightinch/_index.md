---
title: "Cells.GetViewRowHeightInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Restituisce l'altezza di una riga specificata nell'unità di pollici"
type: docs
url: /it/net/aspose.cells/cells/getviewrowheightinch/
---
## Cells.GetViewRowHeightInch method

Restituisce l'altezza di una riga specificata in unità di pollici.

```csharp
public double GetViewRowHeightInch(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga |

### Valore di ritorno

Altezza della riga

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetViewRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'altezza personalizzata della riga per la riga 2 in pollici
            worksheet.Cells.SetRowHeightInch(2, 1.5);

            try
            {
                // Chiama GetViewRowHeightInch con il parametro indice della riga
                double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
                
                // Visualizza il risultato e verifica che l'altezza corrisponda al valore impostato
                Console.WriteLine($"View row height of row 2: {rowHeight} inches");
                
                // Dimostra l'effetto aggiungendo contenuto di esempio
                worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
                worksheet.Cells.SetColumnWidthInch(0, 15);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
            }
            
            // Salva la cartella di lavoro modificata
            workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


