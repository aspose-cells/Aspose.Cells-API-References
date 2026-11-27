---
title: "AutoFilter.Sorter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-egenskap. Hämtar datasorteringsverktyget"
type: docs
url: /sv/net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Hämtar datasorteringen.

```csharp
public DataSorter Sorter { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertySorterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Skapa autofilterområde
            worksheet.AutoFilter.Range = "A1:B4";

            // Hämta autofiltret
            AutoFilter filter = worksheet.AutoFilter;

            // Applicera filter
            filter.Filter(1, "10");

            // Sortera med Sorter-egenskapen
            filter.Sorter.Sort();

            // Spara arbetsboken
            workbook.Save("AutoFilterPropertySorterDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


