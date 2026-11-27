---
title: "CustomFilter.Criteria"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomFilter-egenskap. Hämtar och anger kriterierna"
type: docs
url: /sv/net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

Hämtar och anger kriterierna.

```csharp
public object Criteria { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(5);
            worksheet.Cells["A5"].PutValue(9);
            worksheet.Cells["A6"].PutValue(3);

            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Lägg till anpassat filter
            int fieldIndex = 0;
            autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
            
            // Hämta filterkolumnen och visa kriterierna
            FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Console.WriteLine("Filter Criteria: " + cf.Criteria);
            
            // Uppdatera filtret
            autoFilter.Refresh();
            
            // Spara arbetsboken
            workbook.Save("CustomFilterExample.xlsx");
        }
    }
}
```

### Se även

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


