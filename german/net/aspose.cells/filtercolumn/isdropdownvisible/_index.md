---
title: "FilterColumn.IsDropdownVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn‑Eigenschaft. Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist"
type: docs
url: /de/net/aspose.cells/filtercolumn/isdropdownvisible/
---
## FilterColumn.IsDropdownVisible property

Gibt an, ob die AutoFilter-Schaltfläche für diese Spalte sichtbar ist.

```csharp
public bool IsDropdownVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyIsDropdownVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["A4"].PutValue("Fruit");

            // AutoFilter anwenden
            sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string

            // Ermitteln Sie die Filterspalte
            FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

            // Dropdown zunächst anzeigen
            filterColumn.IsDropdownVisible = true;
            Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");

            // Dropdown ausblenden
            filterColumn.IsDropdownVisible = false;
            Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");

            // Speichere die Arbeitsmappe
            workbook.Save("FilterColumnDropdownDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


