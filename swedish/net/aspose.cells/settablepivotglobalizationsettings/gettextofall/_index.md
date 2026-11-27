---
title: "SettablePivotGlobalizationSettings.GetTextOfAll"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings‑metod. Hämtar texten för etiketten All i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextofall/
---
## SettablePivotGlobalizationSettings.GetTextOfAll method

Hämtar texten för etiketten "(All)" i pivottabellen.

```csharp
public override string GetTextOfAll()
```

### Returvärde

Texten för etiketten "(All)"

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfAllDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(15);

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa globaliseringsinställningar
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();
            settings.SetTextOfAll("(All Items)");

            try
            {
                // Hämta den aktuella texten för etiketten "(All)"
                string currentText = settings.GetTextOfAll();
                Console.WriteLine($"Current text of '(All)' label: {currentText}");

                // Uppdatera pivottabellen med nya inställningar
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfAll method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodGetTextOfAllDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


