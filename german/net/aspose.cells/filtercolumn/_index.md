---
title: "Klasse FilterColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FilterColumn‑Klasse. Stellt einen Filter für eine einzelne Spalte oder eine Spalte in der Tabelle dar."
type: docs
url: /de/net/aspose.cells/filtercolumn/
---
## FilterColumn class

Stellt einen Filter für eine einzelne Spalte oder eine Spalte in der Tabelle dar.

```csharp
public class FilterColumn
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ColorFilter](../../aspose.cells/filtercolumn/colorfilter/) { get; } | Ruft [`ColorFilter`](../colorfilter/) zum Filtern von Daten nach Farbe ab. |
| [CustomFilters](../../aspose.cells/filtercolumn/customfilters/) { get; set; } | Ruft [`CustomFilterCollection`](../customfiltercollection/) zum Filtern von Daten nach benutzerdefinierten Kriterien ab. |
| [DynamicFilter](../../aspose.cells/filtercolumn/dynamicfilter/) { get; } | Ruft [`DynamicFilter`](./dynamicfilter/) zum Filtern mit dynamischen Kriterien ab. |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | Liest und setzt den Spaltenversatz im Bereich. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | (**Obsolete.**) Liest und setzt die Bedingung für das Filtern von Daten. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | Liest und setzt den Typ der Datenfilterung. |
| [FilterValues](../../aspose.cells/filtercolumn/filtervalues/) { get; } | Liest [`FilterValueCollection`](../filtervaluecollection/) zum Filtern von Daten nach Beschriftungen oder Datum/Uhrzeit. |
| [IconFilter](../../aspose.cells/filtercolumn/iconfilter/) { get; } | Liest [`IconFilter`](./iconfilter/) zum Filtern von Daten nach Symbol. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | Gibt an, ob die AutoFilter-Schaltfläche für diese Spalte sichtbar ist. |
| [MultipleFilters](../../aspose.cells/filtercolumn/multiplefilters/) { get; set; } | (**Obsolete.**) Liest [`MultipleFilterCollection`](../multiplefiltercollection/) zum Filtern von Daten nach Beschriftungen oder Datum/Uhrzeit. |
| [Top10Filter](../../aspose.cells/filtercolumn/top10filter/) { get; } | Liest [`Top10Filter`](./top10filter/) zum Filtern von Daten nach Rang. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SelectAll](../../aspose.cells/filtercolumn/selectall/)() | Wählt alles aus. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;

namespace AsposeCellsExamples
{
    public class FilterColumnDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["A4"].PutValue("Doe");

            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(35);

            // AutoFilter auf den Bereich anwenden
            sheet.AutoFilter.SetRange(0, 0, 3);

            // Füge einen Filter zur ersten Spalte (Name) hinzu
            sheet.AutoFilter.AddFilter(0, "John");

            // Füge einen Filter zur zweiten Spalte (Alter) hinzu
            sheet.AutoFilter.AddFilter(1, "30");

            // Aktualisiere den Filter, um ihn anzuwenden
            sheet.AutoFilter.Refresh();

            // Greife auf die FilterColumnCollection zu
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Greife auf die erste FilterColumn zu
            FilterColumn filterColumn = filterColumns[0];

            // Zeige Eigenschaften der FilterColumn an
            Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
            Console.WriteLine($"Filter: {filterColumn.Filter}");
            Console.WriteLine($"FilterType: {filterColumn.FilterType}");
            Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");

            // Speichere die Arbeitsmappe
            workbook.Save("FilterColumnDemo.xlsx");
            workbook.Save("FilterColumnDemo.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


