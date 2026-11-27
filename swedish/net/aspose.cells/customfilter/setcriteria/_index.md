---
title: "CustomFilter.SetCriteria"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomFilter-metod. Sätter filterkriterierna"
type: docs
url: /sv/net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

Anger filterkriterierna.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filterOperator | FilterOperatorType | filteroperatortyp |
| kriterier | Object | filterkriterievärde |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // Applicera ett anpassat filter för att få en CustomFilter‑instans
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Hämta det första anpassade filtret från filterkollektionen
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Ange kriterier med SetCriteria-metoden
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // Visa de angivna kriterierna
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Spara arbetsboken
                workbook.Save("SetCriteriaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


