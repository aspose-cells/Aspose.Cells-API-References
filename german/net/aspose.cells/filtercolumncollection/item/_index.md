---
title: "FilterColumnCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumnCollection-Eigenschaft. Gibt das FilterColumn-Objekt im speziellen Feld zurück"
type: docs
url: /de/net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

Gibt das [`FilterColumn`](../../filtercolumn/) Objekt im speziellen Feld zurück.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| fieldIndex | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |

### Rückgabewert

Gibt das [`FilterColumn`](../../filtercolumn/) Objekt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["A5"].PutValue("Date");

            // Auto-Filter anwenden
            sheet.AutoFilter.Range = "A1:A5";
            sheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "e");

            // Zugriff auf Filter über die Item-Eigenschaft
            AutoFilter filter = sheet.AutoFilter;
            FilterColumn filterColumn = filter.FilterColumns[0]; // Using Item property
            CustomFilterCollection customFilters = (CustomFilterCollection)filterColumn.Filter;
            CustomFilter firstFilter = customFilters[0];

            // Filtereigenschaften anzeigen
            Console.WriteLine("Filter Operator Type: " + firstFilter.FilterOperatorType);
            Console.WriteLine("Filter Criteria: " + firstFilter.Criteria);

            // Filter ändern
            firstFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("\nModified Filter Operator Type: " + firstFilter.FilterOperatorType);

            // Speichere die Arbeitsmappe
            wb.Save("FilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


