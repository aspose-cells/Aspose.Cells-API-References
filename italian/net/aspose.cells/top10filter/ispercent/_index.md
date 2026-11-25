---
title: "Top10Filter.IsPercent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Top10Filter. Indica se filtrare o meno per valore percentuale della colonna"
type: docs
url: /it/net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

Indica se filtrare o meno per valore percentuale della colonna

```csharp
public bool IsPercent { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsPercentDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Applica filtro top 10 (non percentuale)
            worksheet.AutoFilter.Range = "A1:J10";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Ottieni il filtro e dimostra la proprietà IsPercent
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output False

            // Applica filtro top 10 percentuale
            worksheet.AutoFilter.FilterTop10(1, true, true, 20);
            filter = worksheet.AutoFilter.FilterColumns[1].Filter as Top10Filter;
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output True
        }
    }
}
```

### Vedi anche

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


