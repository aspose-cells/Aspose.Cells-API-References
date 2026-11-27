---
title: "SettablePivotGlobalizationSettings.SetTextOfMultipleItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metoden. Ställer in texten för etiketten Multiple Items i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofmultipleitems/
---
## SettablePivotGlobalizationSettings.SetTextOfMultipleItems method

Ställer in texten för etiketten "(Multiple Items)" i PivotTable.

```csharp
public void SetTextOfMultipleItems(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsWithStringDemo
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
                // Ange anpassad text för etiketten "(Multiple Items)" i en pivottabell
                settings.SetTextOfMultipleItems("(Multiple Items Edited)");

                // Hämta och visa den uppdaterade texten
                string currentText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Current text of '(Multiple Items)' label: {currentText}");

                // (Valfritt) Spara arbetsboken – ingen pivottabell krävs för den här demonstrationen
                workbook.Save("SetTextOfMultipleItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


