---
title: "FilterColumn.CustomFilters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn-Eigenschaft. Liefert CustomFilterCollection zum Filtern von Daten nach benutzerdefinierten Kriterien"
type: docs
url: /de/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

Liefert [`CustomFilterCollection`](../../customfiltercollection/) zum Filtern von Daten nach benutzerdefinierten Kriterien.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### Hinweise

HINWEIS: Dieser Setter dieser Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft [`FilterType`](../filtertype/) und setzen Sie sie auf CustomFilters. Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Fügen Sie Beispieldaten hinzu
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // Auto-Filter anwenden
                worksheet.AutoFilter.Range = "A1:A6";

                // Ermitteln Sie die Filterspalte
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Erstellen und setzen Sie benutzerdefinierte Filter mit der Methode AutoFilter.Custom
                // Erster Filter: beginnt mit "A"
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // Zweiter Filter: endet mit "y" (UND-Beziehung)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // Abrufen Sie die benutzerdefinierten Filter aus der Filterspalte
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // Zeigen Sie die Informationen zu den benutzerdefinierten Filtern an
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // Hinweis: CustomFilterCollection stellt einzelne Filter nicht direkt bereit
                // über einen Indexer, sodass wir nur die Sammlungs‑Eigenschaften anzeigen können
                Console.WriteLine("Custom filters have been applied to the column.");

                // Speichere die Arbeitsmappe
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
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

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


