---
title: "SettableChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings‑metod. Hämtar namnet på minskning för legend"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/
---
## SettableChartGlobalizationSettings.GetLegendDecreaseName method

Hämtar namnet på Decrease för Legend.

```csharp
public override string GetLegendDecreaseName()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till enkel data för kontext (valfritt)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Skapa ett diagram (valfritt, bara för att ha en komplett arbetsbok)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Instansiera objektet för globaliseringsinställningar
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Ställ in en anpassad minskningsetikett för legend
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Hämta etiketten med GetLegendDecreaseName
                string legendDecreaseName = settings.GetLegendDecreaseName();

                Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

                // Spara arbetsboken (inställningarna är inte direkt kopplade till chart i den här demonstrationen)
                workbook.Save("GetLegendDecreaseNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendDecreaseName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


