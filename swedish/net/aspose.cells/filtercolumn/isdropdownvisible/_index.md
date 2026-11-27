---
title: "FilterColumn.IsDropdownVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn-egenskap. Anger om AutoFilter-knappen för den här kolumnen är synlig"
type: docs
url: /sv/net/aspose.cells/filtercolumn/isdropdownvisible/
---
## FilterColumn.IsDropdownVisible property

Anger om AutoFilter-knappen för den här kolumnen är synlig.

```csharp
public bool IsDropdownVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyIsDropdownVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["A4"].PutValue("Fruit");

            // Applicera AutoFilter
            sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string

            // Hämta filterkolumnen
            FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

            // Visa rullgardinsmenyn initialt
            filterColumn.IsDropdownVisible = true;
            Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");

            // Dölj rullgardinsmenyn
            filterColumn.IsDropdownVisible = false;
            Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");

            // Spara arbetsboken
            workbook.Save("FilterColumnDropdownDemo.xlsx");
        }
    }
}
```

### Se även

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


