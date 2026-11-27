---
title: "Metered.GetConsumptionQuantity"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Metered method. Hämtar konsumtionsfilens storlek"
type: docs
url: /sv/net/aspose.cells/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Hämtar förbrukningsfilens storlek

```csharp
public static decimal GetConsumptionQuantity()
```

### Returvärde

konsumtionskvantitet

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionQuantityDemo
    {
        public static void Run()
        {
            // Skapa en metered-instans
            Metered metered = new Metered();

            try
            {
                // Ställ in metered-nycklar (ersätt med faktiska nycklar i verklig användning)
                metered.SetMeteredKey("your-public-key", "your-private-key");

                // Hämta förbrukningskvantitet
                decimal consumptionQuantity = Metered.GetConsumptionQuantity();

                // Visa resultatet
                Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");

                // Skapa en arbetsbok för att demonstrera den mätade användningen
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Lägg till lite data för att visa att arbetsboken är funktionell
                worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
                worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");

                // Spara arbetsboken
                workbook.Save("MeteredConsumptionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in metered operation: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


