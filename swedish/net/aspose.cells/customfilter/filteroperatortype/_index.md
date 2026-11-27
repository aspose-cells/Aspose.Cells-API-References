---
title: "CustomFilter.FilterOperatorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomFilter-egenskap. Hämtar och sätter filteroperator-typen"
type: docs
url: /sv/net/aspose.cells/customfilter/filteroperatortype/
---
## CustomFilter.FilterOperatorType property

Hämtar och anger filteroperatorns typ.

```csharp
public FilterOperatorType FilterOperatorType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Mike");
            worksheet.Cells["A5"].PutValue("Emily");

            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Applicera anpassat filter med Contains-operatorn
            filter.Custom(0, FilterOperatorType.Contains, "e");
            
            // Hämta det första anpassade filtret
            CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
            
            // Demonstrera egenskapen FilterOperatorType
            Console.WriteLine("Initial Filter Operator: " + customFilter.FilterOperatorType);
            Console.WriteLine("Criteria: " + customFilter.Criteria);
            
            // Ändra filteroperator-typen
            customFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
            
            // Spara arbetsboken
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


