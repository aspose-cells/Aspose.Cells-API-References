---
title: "SettablePivotGlobalizationSettings.SetTextOfEmptyData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings‑metod. Anger texten för den tomma etiketten i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofemptydata/
---
## SettablePivotGlobalizationSettings.SetTextOfEmptyData method

Ställer in texten för etiketten "(blank)" i PivotTable.

```csharp
public void SetTextOfEmptyData(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten för tom data |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfEmptyDataWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata (valfritt, bara för sammanhang)
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
                // Ange anpassad text för tomma dataceller i en pivottabell
                settings.SetTextOfEmptyData("(no data)");

                // Verifiera ändringen
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Custom text for empty data: {emptyDataText}");

                // (Valfritt) Spara arbetsboken – även om vi inte skapade en pivottabell,
                // detta visar att arbetsboken fortfarande kan sparas efter att inställningarna har manipulerats.
                workbook.Save("SetTextOfEmptyDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


