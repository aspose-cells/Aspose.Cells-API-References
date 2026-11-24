---
title: "FilterColumn.MultipleFilters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn-Eigenschaft. Gibt MultipleFilterCollection zum Filtern von Daten nach Labels oder Datum/Uhrzeit zurück"
type: docs
url: /de/net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

Gibt [`MultipleFilterCollection`](../../multiplefiltercollection/) zum Filtern von Daten nach Labels oder Datum/Uhrzeit zurück.

```csharp
[Obsolete("Use FilterColumn.FilterValues instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MultipleFilterCollection MultipleFilters { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die FilterColumn.FilterValues-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Juni 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Fügen Sie Beispieldaten hinzu
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // AutoFilter auf den Bereich anwenden
                worksheet.AutoFilter.Range = "A1:A5";

                // Erste Filterspalte abrufen
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // MultipleFilters erstellen und festlegen
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // Weisen Sie die MultipleFilters der Filterspalte zu
                filterColumn.MultipleFilters = multipleFilters;

                // MultipleFilters-Eigenschaften anzeigen
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // Speichere die Arbeitsmappe
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


