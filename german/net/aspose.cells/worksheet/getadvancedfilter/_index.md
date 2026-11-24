---
title: "Worksheet.GetAdvancedFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Ruft die Einstellungen des erweiterten Filters ab"
type: docs
url: /de/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

Liest die Einstellungen des erweiterten Filters.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Richten Sie Daten für die Filterung ein
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // Richten Sie den Kriterienbereich ein
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // Wenden Sie den erweiterten Filter an
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // Holen Sie den erweiterten Filter
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // Geben Sie die Filterbereiche aus
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### Siehe auch

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


