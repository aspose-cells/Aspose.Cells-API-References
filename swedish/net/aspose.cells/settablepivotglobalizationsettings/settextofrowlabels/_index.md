---
title: "SettablePivotGlobalizationSettings.SetTextOfRowLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metoden. Anger texten för Row Labels-etiketten i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofrowlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfRowLabels method

Ställer in texten för etiketten "Row Labels" i PivotTable.

```csharp
public void SetTextOfRowLabels(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten för radetiketter |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för sammanhang
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Skapa globaliseringsinställningar
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            SettablePivotGlobalizationSettings pivotSettings = new SettablePivotGlobalizationSettings();
            globalizationSettings.PivotSettings = pivotSettings;

            try
            {
                // Ange anpassad text för "Row Labels"
                pivotSettings.SetTextOfRowLabels("Custom Row Labels");

                // Verifiera ändringen
                string rowLabelsText = pivotSettings.GetTextOfRowLabels();
                Console.WriteLine($"Row Labels text after change: {rowLabelsText}");

                // Applicera inställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Spara arbetsboken
                workbook.Save("SetTextOfRowLabelsDemo.xlsx");
                Console.WriteLine("SetTextOfRowLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


