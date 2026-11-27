---
title: "SettableChartGlobalizationSettings.SetAxisTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings metod. Anger namnet på titel för axel"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/setaxistitlename/
---
## SettableChartGlobalizationSettings.SetAxisTitleName method

Ställer in namnet på Title för Axis.

```csharp
public void SetAxisTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetAxisTitleNameDemo
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

                // Ange ett anpassat axeltitelnamn
                settings.SetAxisTitleName("Custom Axis Title");

                // Verifiera inställningen genom att hämta axeltitelns namn
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Spara arbetsboken
                workbook.Save("SetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


