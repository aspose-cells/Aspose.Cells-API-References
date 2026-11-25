---
title: "Worksheet.GetAdvancedFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Ottiene le impostazioni del filtro avanzato"
type: docs
url: /it/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

Ottiene le impostazioni del filtro avanzato.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Configura i dati per il filtraggio
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // Configura l'intervallo dei criteri
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // Applica il filtro avanzato
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // Ottieni il filtro avanzato
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // Restituisci gli intervalli del filtro
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### Vedi anche

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


