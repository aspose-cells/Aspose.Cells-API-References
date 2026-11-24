---
title: "AdvancedFilter.ListRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AdvancedFilter-Eigenschaft. Gibt den Listenbereich dieses erweiterten Filters zurück"
type: docs
url: /de/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

Ermittelt den Listbereich dieses erweiterten Filters.

```csharp
public string ListRange { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten befüllen
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // Erweiterten Filter einrichten
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange ist schreibgeschützt und wird beim Erstellen des Filters automatisch festgelegt
            // Wir können es nur lesen, nicht direkt setzen
            
            // ListRange anzeigen (zeigt den automatisch ermittelten Bereich)
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // Speichere die Arbeitsmappe
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


