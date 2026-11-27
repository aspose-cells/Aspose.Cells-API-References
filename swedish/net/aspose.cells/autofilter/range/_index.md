---
title: "AutoFilter.Range"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-egenskap. Representerar det område som den angivna AutoFilter gäller för"
type: docs
url: /sv/net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Representerar det område som den angivna AutoFilter gäller för.

```csharp
public string Range { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["A5"].PutValue("Item4");

            // Applicera autofilter på området A1:A5
            sheet.AutoFilter.Range = "A1:A5";

            // Visa autofilterområdet
            Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);

            // Spara arbetsboken
            workbook.Save("AutoFilterRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


