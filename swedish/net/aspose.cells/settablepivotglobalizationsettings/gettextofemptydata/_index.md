---
title: "SettablePivotGlobalizationSettings.GetTextOfEmptyData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings‑metod. Hämtar texten för den tomma etiketten i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextofemptydata/
---
## SettablePivotGlobalizationSettings.GetTextOfEmptyData method

Hämtar texten för etiketten "(blank)" i pivottabellen.

```csharp
public override string GetTextOfEmptyData()
```

### Returvärde

Texten för tom data

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa en instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Hämta standardtexten för tom data
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Default text for empty data: '{emptyDataText}'");

                // Ange en anpassad text för tom data
                settings.SetTextOfEmptyData("No Data Available");

                // Hämta den uppdaterade texten för tom data
                string updatedEmptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Updated text for empty data: '{updatedEmptyDataText}'");

                // Applicera inställningar på arbetsboken
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
                globalizationSettings.PivotSettings = settings;
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Spara arbetsboken
                workbook.Save("GetTextOfEmptyDataDemo.xlsx");
                Console.WriteLine("GetTextOfEmptyData method demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


