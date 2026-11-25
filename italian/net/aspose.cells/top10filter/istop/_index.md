---
title: "Top10Filter.IsTop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Top10Filter. Indica se filtrare o meno per ordine top"
type: docs
url: /it/net/aspose.cells/top10filter/istop/
---
## Top10Filter.IsTop property

Indica se filtrare o meno per ordine superiore

```csharp
public bool IsTop { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsTopDemo
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
            }

            // Applica filtro top 5
            worksheet.AutoFilter.Range = "B6:B16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Ottieni il filtro e verifica la proprietà IsTop
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop); // Should output "True"
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output "False"
            
            // Aggiorna filtro e verifica le righe nascoste
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Vedi anche

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


