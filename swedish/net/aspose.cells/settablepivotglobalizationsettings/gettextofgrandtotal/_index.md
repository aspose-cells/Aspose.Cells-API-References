---
title: "SettablePivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings‑metod. Hämtar texten för etiketten Grand Total i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextofgrandtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfGrandTotal method

Hämtar texten för etiketten "Grand Total" i pivottabellen.

```csharp
public override string GetTextOfGrandTotal()
```

### Returvärde

Texten för etiketten "Grand Total"

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok (bara för sammanhang)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample");

            // Instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ändra standardtexten för "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Hämta den aktuella "Grand Total"-texten
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Spara arbetsboken (ingen pivottabell skapas, men filen sparas för att bevisa körning)
                workbook.Save("GetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


