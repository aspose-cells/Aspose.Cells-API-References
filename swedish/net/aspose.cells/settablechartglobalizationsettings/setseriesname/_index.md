---
title: "SettableChartGlobalizationSettings.SetSeriesName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings-metoden. Anger namnet på serien i diagrammet"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/setseriesname/
---
## SettableChartGlobalizationSettings.SetSeriesName method

Ställer in namnet på Series i Chart.

```csharp
public void SetSeriesName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetSeriesNameWithStringDemo
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

                // Ange ett anpassat serienamn med SetSeriesName och en strängparameter
                settings.SetSeriesName("Custom Series Label");

                // Verifiera inställningen genom att hämta serienamnet
                string seriesName = settings.GetSeriesName();
                Console.WriteLine($"Series name set to: {seriesName}");

                // Spara arbetsboken
                workbook.Save("SetSeriesNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetSeriesName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


