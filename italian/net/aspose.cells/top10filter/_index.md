---
title: "Classe Top10Filter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Top10Filter. Rappresenta la percentuale o il numero dei primi N elementi da filtrare"
type: docs
url: /it/net/aspose.cells/top10filter/
---
## Top10Filter class

Rappresenta i primi N (percentuale o numero di elementi) da filtrare.

```csharp
public class Top10Filter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Obsolete.**) Il valore effettivo della cella nell'intervallo che viene utilizzato per eseguire il confronto per questo filtro. Questo è il valore di cache durante il processo di aggiornamento. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Indica se filtrare o meno per valore percentuale della colonna |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Indica se filtrare o meno per ordine superiore |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Ottiene e imposta il valore superiore o inferiore da utilizzare come criterio di filtro. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // Applica il filtro automatico e il filtro Top 10
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // Ottieni il Top10Filter e verifica le sue proprietà
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // Aggiorna il filtro e controlla le righe nascoste
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


