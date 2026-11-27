---
title: "SettablePivotGlobalizationSettings.SetTextOfGrandTotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metoden. Ställer in texten för Grand Total-etiketten i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

Ställer in texten för etiketten "Grand Total" i PivotTable.

```csharp
public void SetTextOfGrandTotal(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok (endast kontext)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ange en anpassad text för etiketten "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Hämta den uppdaterade etiketttexten för att verifiera ändringen
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Spara arbetsboken bara för att demonstrera att koden körs utan fel
                workbook.Save("SetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


