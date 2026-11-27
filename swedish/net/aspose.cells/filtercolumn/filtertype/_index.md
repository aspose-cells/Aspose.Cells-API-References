---
title: "FilterColumn.FilterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn-egenskapen. Hämtar och anger typen av filtrering av data"
type: docs
url: /sv/net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

Hämtar och anger typen av filtrering av data.

```csharp
public FilterType FilterType { get; set; }
```

### Anmärkningar

Det motsvarande filterobjektet kommer att skapas när denna egenskap sätts och motsvarande egenskap bör användas för att hämta filterobjektet på lämpligt sätt:

| **FilterType** | **Property** |
| --- | --- |
| MultipleFilters | [`FilterValues`](../filtervalues/) |
| CustomFilters | [`CustomFilters`](../customfilters/) |
| ColorFilter | [`ColorFilter`](../colorfilter/) |
| DynamicFilter | [`DynamicFilter`](../dynamicfilter/) |
| IconFilter | [`IconFilter`](../iconfilter/) |
| Top10 | [`Top10Filter`](../top10filter/) |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("HR");
            sheet.Cells["A3"].PutValue("IT");
            sheet.Cells["A4"].PutValue("Finance");

            sheet.Cells["B1"].PutValue("Employees");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(15);
            sheet.Cells["B4"].PutValue(8);

            // Tillämpa auto-filter med strängintervall
            sheet.AutoFilter.Range = "A1:B4";

            // Lägg till olika filtertyper för att demonstrera FilterType-egenskapen
            sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
            sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter

            // Hämta filterkolumner
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Visa FilterType för varje kolumn
            for (int i = 0; i < filterColumns.Count; i++)
            {
                FilterColumn filterColumn = filterColumns[i];
                Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
            }

            // Spara arbetsboken
            workbook.Save("FilterTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


