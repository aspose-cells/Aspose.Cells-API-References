---
title: "Class CustomFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CustomFilter‑klass. Representerar det anpassade filtret"
type: docs
url: /sv/net/aspose.cells/customfilter/
---
## CustomFilter class

Representerar det anpassade filtret.

```csharp
public class CustomFilter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | Hämtar och anger kriterierna. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | Hämtar och anger filteroperatorns typ. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | Anger filterkriterierna. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till exempeldata i kalkylbladet
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // Applicera autofilter på intervallet
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // Applicera ett anpassat filter för att få en CustomFilter‑instans
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Hämta det första anpassade filtret från filterkollektionen
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Visa filteregenskaperna
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Modifiera filterkriterierna med SetCriteria‑metoden
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // Visa de uppdaterade filteregenskaperna
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // Spara arbetsboken
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


