---
title: "SettablePivotGlobalizationSettings.SetTextOfProtectedName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metoden. Ställer in texten för ett specifikt skyddat namn"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofprotectedname/
---
## SettablePivotGlobalizationSettings.SetTextOfProtectedName method

Ställer in texten för ett specifikt skyddat namn.

```csharp
public void SetTextOfProtectedName(string protectedName, string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| protectedName | String | Det skyddade namnet i pivottabellen. |
| text | String | De lokala skyddade namnen i pivottabellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata för sammanhang
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Skapa en instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ange anpassad text för ett skyddat namn
                settings.SetTextOfProtectedName("Sum", "Custom Sum Label");

                // Verifiera ändringen genom att hämta den aktuella texten
                string currentText = settings.GetTextOfProtectedName("Sum");
                Console.WriteLine($"Text for protected name 'Sum': {currentText}");

                // Spara arbetsboken för att demonstrera en lyckad körning
                workbook.Save("SetTextOfProtectedNameDemo.xlsx");
                Console.WriteLine("SetTextOfProtectedName method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


