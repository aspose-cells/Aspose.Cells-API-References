---
title: "Klass FilterColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FilterColumn-klass. Representerar ett filter för en enskild kolumn eller en kolumn i tabellen"
type: docs
url: /sv/net/aspose.cells/filtercolumn/
---
## FilterColumn class

Representerar ett filter för en enskild kolumn eller en kolumn i tabellen.

```csharp
public class FilterColumn
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ColorFilter](../../aspose.cells/filtercolumn/colorfilter/) { get; } | Hämtar [`ColorFilter`](../colorfilter/) för att filtrera data efter färg. |
| [CustomFilters](../../aspose.cells/filtercolumn/customfilters/) { get; set; } | Hämtar [`CustomFilterCollection`](../customfiltercollection/) för att filtrera data efter anpassade kriterier. |
| [DynamicFilter](../../aspose.cells/filtercolumn/dynamicfilter/) { get; } | Hämtar [`DynamicFilter`](./dynamicfilter/) för att filtrera med dynamiska kriterier. |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | Hämtar och anger kolumnförskjutningen i intervallet. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | (**Obsolete.**) Hämtar och anger villkoret för filtrering av data. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | Hämtar och anger typen av filtrering av data. |
| [FilterValues](../../aspose.cells/filtercolumn/filtervalues/) { get; } | Hämtar [`FilterValueCollection`](../filtervaluecollection/) för att filtrera data efter etiketter eller datum/tid. |
| [IconFilter](../../aspose.cells/filtercolumn/iconfilter/) { get; } | Hämtar [`IconFilter`](./iconfilter/) för att filtrera data efter ikon. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | Anger om AutoFilter-knappen för den här kolumnen är synlig. |
| [MultipleFilters](../../aspose.cells/filtercolumn/multiplefilters/) { get; set; } | (**Föråldrad.**) Hämtar [`MultipleFilterCollection`](../multiplefiltercollection/) för att filtrera data efter etiketter eller datum/tid. |
| [Top10Filter](../../aspose.cells/filtercolumn/top10filter/) { get; } | Hämtar [`Top10Filter`](./top10filter/) för att filtrera data efter dataens rang. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SelectAll](../../aspose.cells/filtercolumn/selectall/)() | Väljer alla. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["A4"].PutValue("Doe");

            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(35);

            // Tillämpa AutoFilter på intervallet
            sheet.AutoFilter.SetRange(0, 0, 3);

            // Lägg till ett filter i den första kolumnen (Name)
            sheet.AutoFilter.AddFilter(0, "John");

            // Lägg till ett filter i den andra kolumnen (Age)
            sheet.AutoFilter.AddFilter(1, "30");

            // Uppdatera filtret för att tillämpa det
            sheet.AutoFilter.Refresh();

            // Få åtkomst till FilterColumnCollection
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Få åtkomst till den första FilterColumn
            FilterColumn filterColumn = filterColumns[0];

            // Visa egenskaper för FilterColumn
            Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
            Console.WriteLine($"Filter: {filterColumn.Filter}");
            Console.WriteLine($"FilterType: {filterColumn.FilterType}");
            Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");

            // Spara arbetsboken
            workbook.Save("FilterColumnDemo.xlsx");
            workbook.Save("FilterColumnDemo.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


