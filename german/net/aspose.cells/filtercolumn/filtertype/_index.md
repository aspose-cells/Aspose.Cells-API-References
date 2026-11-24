---
title: "FilterColumn.FilterType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn-Eigenschaft. Gibt den Typ der Datenfilterung zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

Liest und setzt den Typ der Datenfilterung.

```csharp
public FilterType FilterType { get; set; }
```

### Hinweise

Das entsprechende Filterobjekt wird erstellt, wenn diese Eigenschaft gesetzt wird, und die zugehörige Eigenschaft sollte verwendet werden, um das Filterobjekt entsprechend zu erhalten:

| **FilterType** | **Property** |
| --- | --- |
| MultipleFilters | [`FilterValues`](../filtervalues/) |
| CustomFilters | [`CustomFilters`](../customfilters/) |
| ColorFilter | [`ColorFilter`](../colorfilter/) |
| DynamicFilter | [`DynamicFilter`](../dynamicfilter/) |
| IconFilter | [`IconFilter`](../iconfilter/) |
| Top10 | [`Top10Filter`](../top10filter/) |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("HR");
            sheet.Cells["A3"].PutValue("IT");
            sheet.Cells["A4"].PutValue("Finance");

            sheet.Cells["B1"].PutValue("Employees");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(15);
            sheet.Cells["B4"].PutValue(8);

            // Auto-Filter mit Zeichenfolgenbereich anwenden
            sheet.AutoFilter.Range = "A1:B4";

            // Verschiedene Filtertypen hinzufügen, um die FilterType property zu demonstrieren
            sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
            sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter

            // Filterspalten abrufen
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // FilterType für jede Spalte anzeigen
            for (int i = 0; i < filterColumns.Count; i++)
            {
                FilterColumn filterColumn = filterColumns[i];
                Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("FilterTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


