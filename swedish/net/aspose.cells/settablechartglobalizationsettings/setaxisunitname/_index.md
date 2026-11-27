---
title: "SettableChartGlobalizationSettings.SetAxisUnitName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings‑metod. Ställer in namnet på axelens enhet"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/setaxisunitname/
---
## SettableChartGlobalizationSettings.SetAxisUnitName method

Ställer in namnet på Axis Unit.

```csharp
public void SetAxisUnitName(DisplayUnitType type, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | DisplayUnitType | Enhetstypen för att visa axelns etiketter. |
| namn | String | lokalt beroende namn |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetAxisUnitNameWithDisplayUnitTypeStringDemo
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

                // Ange anpassade namn för axelns enheter för olika DisplayUnitType‑värden
                settings.SetAxisUnitName(DisplayUnitType.Thousands, "K");
                settings.SetAxisUnitName(DisplayUnitType.Millions, "M");
                settings.SetAxisUnitName(DisplayUnitType.Percentage, "Pct");

                // Verifiera inställningarna genom att hämta värdena
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // Visa resultaten
                Console.WriteLine($"Thousands unit name set to: {thousandsUnit}");
                Console.WriteLine($"Millions unit name set to: {millionsUnit}");
                Console.WriteLine($"Percentage unit name set to: {percentageUnit}");

                // Spara arbetsboken
                workbook.Save("SetAxisUnitNameDemo.xlsx");
                Console.WriteLine("SetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisUnitName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


