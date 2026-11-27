---
title: "SettableChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings-metoden. Hämtar namnet på ökningen för legend"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/getlegendincreasename/
---
## SettableChartGlobalizationSettings.GetLegendIncreaseName method

Hämtar namnet på increase för Legend.

```csharp
public override string GetLegendIncreaseName()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till minimal data för kontext
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Skapa en instans av SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Ställ in ett anpassat namn för legendökning
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Hämta namnet på legendökningen med GetLegendIncreaseName
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

                // Spara arbetsboken
                workbook.Save("GetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


