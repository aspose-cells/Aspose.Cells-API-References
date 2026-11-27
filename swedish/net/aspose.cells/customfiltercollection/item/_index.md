---
title: "CustomFilterCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomFilterCollection-egenskap. Hämtar det anpassade filtret på det specifika indexet"
type: docs
url: /sv/net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

Hämtar det anpassade filtret på det specifika indexet.

```csharp
public CustomFilter this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Skapa en ny CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Åtkomst till egenskapen Item (skrivskyddad) med indexerare
                // Eftersom samlingen är tom kommer vi bara att demonstrera åtkomst till egenskapen
                // I ett verkligt scenario skulle du först lägga till filter på annat sätt
                if (filters.Count > 0)
                {
                    CustomFilter firstFilter = filters[0];
                    Console.WriteLine($"First filter operator: {firstFilter.FilterOperatorType}");
                    Console.WriteLine($"First filter criteria: {firstFilter.Criteria}");
                }
                else
                {
                    Console.WriteLine("No filters in collection to demonstrate Item property");
                }

                // Spara arbetsboken
                workbook.Save("CustomFilterCollectionItemDemo.xlsx");
                Console.WriteLine("CustomFilterCollection Item property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


