---
title: "AdvancedFilter.CriteriaRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AdvancedFilter-Eigenschaft. Gibt den Kriterienbereich dieses erweiterten Filters zurück"
type: docs
url: /de/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Ermittelt den Kriterienbereich dieses erweiterten Filters.

```csharp
public string CriteriaRange { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für den Listbereich bereitstellen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // Beispielkriterien füllen (der Filter verwendet diese bei Anwendung)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // AdvancedFilter-Objekt für das Arbeitsblatt erhalten
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // Die Eigenschaften ListRange, CriteriaRange und CopyToRange sind schreibgeschützt.
                // Die automatisch ermittelten Bereiche anzeigen.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // Arbeitsmappe speichern (optional, nur um zu zeigen, dass die Datei erstellt werden kann)
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


