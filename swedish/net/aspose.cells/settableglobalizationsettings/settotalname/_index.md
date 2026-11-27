---
title: "SettableGlobalizationSettings.SetTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metoden. Ställer in totalnamnet för en specifik funktion"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/settotalname/
---
## SettableGlobalizationSettings.SetTotalName method

Ställer in totalnamnet för en specifik funktion.

```csharp
public void SetTotalName(ConsolidationFunction functionType, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | ConsolidationFunction | Funktionstypen. |
| namn | String | Totalnamnet för funktionen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för konsolidering
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Ange anpassat totalnamn för Sum‑funktionen
                settings.SetTotalName(ConsolidationFunction.Sum, "Custom Sum Total");
                
                // Ange anpassat totalnamn för Average‑funktionen
                settings.SetTotalName(ConsolidationFunction.Average, "Custom Average Total");

                // Applicera inställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                // Verifiera inställningarna genom att hämta tillbaka värdena
                string sumTotalName = settings.GetTotalName(ConsolidationFunction.Sum);
                string avgTotalName = settings.GetTotalName(ConsolidationFunction.Average);

                Console.WriteLine($"Sum total name set to: {sumTotalName}");
                Console.WriteLine($"Average total name set to: {avgTotalName}");

                // Skapa en pivottabell för att demonstrera effekten
                worksheet.Cells["D1"].PutValue("Pivot Table");
                var pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
                var pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Spara arbetsboken
                workbook.Save("SetTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTotalName method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


