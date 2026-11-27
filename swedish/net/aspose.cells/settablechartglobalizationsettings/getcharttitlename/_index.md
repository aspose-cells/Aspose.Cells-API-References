---
title: "SettableChartGlobalizationSettings.GetChartTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings‑metod. Hämtar namnet på diagramrubrik"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/getcharttitlename/
---
## SettableChartGlobalizationSettings.GetChartTitleName method

Hämtar namnet på Chart Title.

```csharp
public override string GetChartTitleName()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetChartTitleNameDemo
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

                // Ställ in ett anpassat diagramrubriknamn
                settings.SetChartTitleName("Custom Chart Title");

                // Hämta diagramrubrikens namn med GetChartTitleName
                string chartTitleName = settings.GetChartTitleName();

                // Visa resultatet
                Console.WriteLine("Chart Title Name: " + chartTitleName);

                // Spara arbetsboken
                workbook.Save("GetChartTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


