---
title: "DynamicFilter.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DynamicFilter property. Hämtar och anger det dynamiska filtervärdet"
type: docs
url: /sv/net/aspose.cells/dynamicfilter/value/
---
## DynamicFilter.Value property

Hämtar och anger värdet för det dynamiska filtret.

```csharp
public object Value { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            // Skapa autofilter
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Visa aktuellt filtervärde
            Console.WriteLine("Current DynamicFilter Value: " + filter.Value);

            // Ändra filtervärdet för att visa datum i april
            filter.Value = new DateTime(2023, 4, 1);
            filter.DynamicFilterType = DynamicFilterType.April;

            // Tillämpa filtret
            worksheet.AutoFilter.Refresh();

            // Spara resultatet
            workbook.Save("DynamicFilterValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


