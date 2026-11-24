---
title: "Klasse AdvancedFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AdvancedFilter Klasse. Stellt die Einstellungen des erweiterten Filters dar."
type: docs
url: /de/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Stellt die Einstellungen des erweiterten Filters dar.

```csharp
public class AdvancedFilter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Ermittelt den Bereich, in den das Ergebnis dieses erweiterten Filters kopiert wird. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Ermittelt den Kriterienbereich dieses erweiterten Filters. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Ermittelt den Listbereich dieses erweiterten Filters. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Beispieldaten für den Listbereich bereitstellen
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // Kriterienbereich bereitstellen
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // Hole die AdvancedFilter-Instanz aus dem Arbeitsblatt
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Zeige die schreibgeschützten Eigenschaften an
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // Speichere die Arbeitsmappe
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


