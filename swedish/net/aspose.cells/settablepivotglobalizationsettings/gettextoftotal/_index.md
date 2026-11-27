---
title: "SettablePivotGlobalizationSettings.GetTextOfTotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metoden. Hämtar texten för Total-etiketten i pivottabellen. Du måste åsidosätta den här metoden när pivottabellen innehåller två eller fler pivottfält i dataområdet."
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextoftotal/
---
## SettablePivotGlobalizationSettings.GetTextOfTotal method

Hämtar texten för etiketten "Total" i PivotTable. Du måste åsidosätta den här metoden när PivotTable innehåller två eller fler PivotFields i dataområdet.

```csharp
public override string GetTextOfTotal()
```

### Returvärde

Texten för etiketten "Total"

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata för sammanhang
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Skapa en instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ange anpassad text för etiketten "Total"
                settings.SetTextOfTotal("Custom Total");

                // Hämta texten för etiketten "Total"
                string totalText = settings.GetTextOfTotal();

                Console.WriteLine($"Text of Total: {totalText}");

                // Spara arbetsboken
                workbook.Save("GetTextOfTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


