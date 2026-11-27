---
title: "SettableChartGlobalizationSettings.SetChartTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings‑metod. Ställer in namnet på diagramrubrik"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/setcharttitlename/
---
## SettableChartGlobalizationSettings.SetChartTitleName method

Ställer in namnet på Chart Title.

```csharp
public void SetChartTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetChartTitleNameDemo
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

                // Anropa SetChartTitleName med en anpassad sträng
                settings.SetChartTitleName("Custom Chart Title");

                // Verifiera inställningen genom att hämta värdet
                string chartTitleName = settings.GetChartTitleName();
                Console.WriteLine("Chart Title Name set to: " + chartTitleName);

                // Spara arbetsboken
                workbook.Save("SetChartTitleNameDemo.xlsx");
                Console.WriteLine("SetChartTitleName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


