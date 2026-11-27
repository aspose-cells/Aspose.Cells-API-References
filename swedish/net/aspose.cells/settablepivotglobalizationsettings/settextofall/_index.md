---
title: "SettablePivotGlobalizationSettings.SetTextOfAll"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metoden. Anger texten för All-etiketten i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofall/
---
## SettablePivotGlobalizationSettings.SetTextOfAll method

Ställer in texten för etiketten "(All)" i PivotTable.

```csharp
public void SetTextOfAll(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | anpassad text |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfAllWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Skapa pivottabell
            var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Skapa globaliseringsinställningar
            var settings = new SettableGlobalizationSettings();
            settings.PivotSettings = new SettablePivotGlobalizationSettings();

            try
            {
                // Anropa SetTextOfAll-metoden för att ändra "(All)"-texten
                ((SettablePivotGlobalizationSettings)settings.PivotSettings).SetTextOfAll("All Products");

                // Applicera inställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;

                Console.WriteLine("SetTextOfAll method executed successfully. Changed '(All)' to 'All Products'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfAll method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfAllDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


