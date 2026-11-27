---
title: "DynamicFilter.MaxValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DynamicFilter property. Hämtar och anger det maximala värdet för det dynamiska filtret"
type: docs
url: /sv/net/aspose.cells/dynamicfilter/maxvalue/
---
## DynamicFilter.MaxValue property

Hämtar och anger det maximala värdet för det dynamiska filtret.

```csharp
public object MaxValue { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempel på numerisk data
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // Skapa autofilter
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Tillämpa dynamiskt filter med intervallkriterier
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Visa aktuellt MaxValue
            Console.WriteLine("Current MaxValue: " + filter.MaxValue);

            // Eftersom DynamicFilterType.Between inte finns kommer vi att använda ett annat tillvägagångssätt
            // Till exempel kan vi använda ett anpassat filter istället
            worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
            worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);

            // Tillämpa filtret
            worksheet.AutoFilter.Refresh();

            // Spara resultatet
            workbook.Save("DynamicFilterMaxValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


