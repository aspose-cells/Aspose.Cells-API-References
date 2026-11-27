---
title: "SettableGlobalizationSettings.GetTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metoden. Hämtar totalnamnet för en specifik funktion"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/gettotalname/
---
## SettableGlobalizationSettings.GetTotalName method

Hämtar totalnamnet för en specifik funktion.

```csharp
public override string GetTotalName(ConsolidationFunction functionType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | ConsolidationFunction | Funktionstypen. |

### Returvärde

Totalnamnet för funktionen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Anropa GetTotalName med ConsolidationFunction.Sum
                string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
                
                // Visa resultatet
                Console.WriteLine($"Total name for Sum function: {totalName}");

                // Lägg till data för att demonstrera effekten (även om GetTotalName inte ändrar kalkylbladet)
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["B1"].PutValue("Total");
                worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
                
                // Beräkna formler
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


