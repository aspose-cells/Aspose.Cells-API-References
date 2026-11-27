---
title: "Metered.GetConsumptionCredit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Metered-metod. Hämtar förbrukningskredit"
type: docs
url: /sv/net/aspose.cells/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Hämtar förbrukningskredit

```csharp
public static decimal GetConsumptionCredit()
```

### Returvärde

konsumtionskvantitet

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionCreditDemo
    {
        public static void Run()
        {
            // Skapa en instans av Metered-klassen
            Metered metered = new Metered();

            try
            {
                // Anropa GetConsumptionCredit-metoden som statisk
                decimal consumptionCredit = Metered.GetConsumptionCredit();
                
                // Visa resultatet
                Console.WriteLine($"Current consumption credit: {consumptionCredit}");
                
                // Skapa en enkel arbetsbok för att demonstrera effekten (även om GetConsumptionCredit inte modifierar arbetsboken)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Lägg till förbrukningskreditinformationen i kalkylbladet
                worksheet.Cells["A1"].PutValue("Consumption Credit:");
                worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
                
                // Spara arbetsboken
                workbook.Save("MeteredGetConsumptionCreditDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error getting consumption credit: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


