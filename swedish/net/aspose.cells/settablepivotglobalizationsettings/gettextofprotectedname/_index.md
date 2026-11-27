---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings‑metod. Hämtar texten för angivet skyddat namn"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

Hämtar texten för angivet skyddat namn.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| protectedName | String | Det skyddade namnet i pivottabellen. |

### Returvärde

De lokala skyddade namnen i pivottabellen.

### Anmärkningar

I Ms Excel är vissa namn inte tillåtna att användas som namn på PivotFields i en pivottabell. De varierar mellan regioner, och användaren kan ange dem explicit enligt den använda regionen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
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
                // Ange en anpassad text för ett skyddat namn
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // Hämta texten för det skyddade namnet
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // Spara arbetsboken
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


