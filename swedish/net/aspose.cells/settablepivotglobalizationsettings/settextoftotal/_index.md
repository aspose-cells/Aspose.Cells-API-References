---
title: "SettablePivotGlobalizationSettings.SetTextOfTotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metoden. Ställer in texten för Total-etiketten i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextoftotal/
---
## SettablePivotGlobalizationSettings.SetTextOfTotal method

Ställer in texten för etiketten "Total" i PivotTable.

```csharp
public void SetTextOfTotal(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | anpassad text |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfTotalWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata för sammanhang
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 200;

            // Skapa en instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Hämta standardtexten "Total"
                string defaultTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Default Total text: {defaultTotalText}");

                // Ange en anpassad text för "Total"
                settings.SetTextOfTotal("Custom Total Label");

                // Verifiera ändringen
                string updatedTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Updated Total text: {updatedTotalText}");

                // Spara arbetsboken
                workbook.Save("SetTextOfTotalDemo.xlsx");
                Console.WriteLine("SetTextOfTotal method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


