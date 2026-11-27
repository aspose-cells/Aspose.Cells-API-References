---
title: "SettablePivotGlobalizationSettings.SetTextOfColumnLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metod. Hämtar texten för etiketten Kolumnrubriker i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

Hämtar texten för etiketten "Column Labels" i pivottabellen.

```csharp
public void SetTextOfColumnLabels(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten för kolumnrubriker |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok (bara för sammanhang)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Skapa en instans av SettablePivotGlobalizationSettings
                SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

                // Ange anpassad text för etiketten "Column Labels"
                string customColumnLabel = "My Column Headers";
                settings.SetTextOfColumnLabels(customColumnLabel);

                // Hämta den aktuella texten för att verifiera ändringen
                string currentLabel = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Column Labels text is now: \"{currentLabel}\"");

                // Spara arbetsboken (ingen pivottabell krävs för denna demo)
                workbook.Save("SetTextOfColumnLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


