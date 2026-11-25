---
title: "AdvancedFilter.ListRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AdvancedFilter. Restituisce l'intervallo di elenco di questo filtro avanzato"
type: docs
url: /it/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

Ottiene l'intervallo dell'elenco di questo filtro avanzato.

```csharp
public string ListRange { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Popola dati di esempio
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // Configura il filtro avanzato
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange è di sola lettura e viene impostato automaticamente durante la creazione del filtro
            // Possiamo solo leggerlo, non impostarlo direttamente
            
            // Visualizza l'intervallo di elenco (mostrerà l'intervallo determinato automaticamente)
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // Salva la cartella di lavoro
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


