---
title: "FilterColumnCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumnCollection-egenskap. Hämtar FilterColumn-objektet vid det specifika fältet"
type: docs
url: /sv/net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

Hämtar [`FilterColumn`](../../filtercolumn/) objektet vid det specifika fältet.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| fieldIndex | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |

### Returvärde

Returnerar [`FilterColumn`](../../filtercolumn/) objektet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["A5"].PutValue("Date");

            // Applicera autofilter
            sheet.AutoFilter.Range = "A1:A5";
            sheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "e");

            // Åtkomst till filter med Item-egenskapen
            AutoFilter filter = sheet.AutoFilter;
            FilterColumn filterColumn = filter.FilterColumns[0]; // Using Item property
            CustomFilterCollection customFilters = (CustomFilterCollection)filterColumn.Filter;
            CustomFilter firstFilter = customFilters[0];

            // Visa filteregenskaper
            Console.WriteLine("Filter Operator Type: " + firstFilter.FilterOperatorType);
            Console.WriteLine("Filter Criteria: " + firstFilter.Criteria);

            // Modifiera filter
            firstFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("\nModified Filter Operator Type: " + firstFilter.FilterOperatorType);

            // Spara arbetsboken
            wb.Save("FilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


