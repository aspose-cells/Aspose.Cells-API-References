---
title: "SettableChartGlobalizationSettings.SetLegendIncreaseName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings‑metod. Ställer in namnet på ökning för legend"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/setlegendincreasename/
---
## SettableChartGlobalizationSettings.SetLegendIncreaseName method

Ställer in namnet på increase för Legend.

```csharp
public void SetLegendIncreaseName(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | lokalt beroende namn |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendIncreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till minimal data för kontext
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Item 1";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Skapa en instans av SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Ställ in ett anpassat namn för legendökning
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Verifiera inställningen genom att hämta värdet
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name set to: " + legendIncreaseName);

                // Spara arbetsboken
                workbook.Save("SetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


