---
title: "SettableChartGlobalizationSettings.SetLegendTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings-metoden. Anger namnet på totalen för legend"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/setlegendtotalname/
---
## SettableChartGlobalizationSettings.SetLegendTotalName method

Ställer in namnet på Total för Legend.

```csharp
public void SetLegendTotalName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetLegendTotalNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till minimal data för kontext
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // Skapa en instans av SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Ange ett anpassat namn för legendens total
                settings.SetLegendTotalName("Custom Total Label");

                // Verifiera inställningen genom att hämta värdet
                string legendTotalName = settings.GetLegendTotalName();
                Console.WriteLine("Legend Total Name set to: " + legendTotalName);

                // Spara arbetsboken
                workbook.Save("SetLegendTotalNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


