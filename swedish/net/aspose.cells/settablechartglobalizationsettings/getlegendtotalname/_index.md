---
title: "SettableChartGlobalizationSettings.GetLegendTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings metod. Hämtar namnet på total för legend"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

Hämtar namnet på Total för Legend.

```csharp
public override string GetLegendTotalName()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Skapa en instans av SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Ange först ett anpassat legendtotalnamn
                settings.SetLegendTotalName("Custom Total Label");

                // Anropa GetLegendTotalName-metoden för att hämta värdet
                string legendTotalName = settings.GetLegendTotalName();

                // Visa resultatet
                Console.WriteLine("Legend Total Name: " + legendTotalName);

                // Spara arbetsboken
                workbook.Save("GetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


