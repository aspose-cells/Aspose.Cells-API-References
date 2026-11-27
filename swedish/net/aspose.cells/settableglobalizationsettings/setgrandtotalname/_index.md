---
title: "SettableGlobalizationSettings.SetGrandTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Anger det totala namnet för en specifik funktion"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setgrandtotalname/
---
## SettableGlobalizationSettings.SetGrandTotalName method

Ställer in det samlade totalnamnet för en specifik funktion.

```csharp
public void SetGrandTotalName(ConsolidationFunction functionType, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | ConsolidationFunction | Funktionstypen. |
| namn | String | Det totala namnet på funktionen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetGrandTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(75);

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Anropa SetGrandTotalName med ConsolidationFunction.Sum och ett anpassat namn
                settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Grand Total");

                // Uppdatera pivottabellen för att tillämpa ändringarna
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Grand total name set to 'Custom Grand Total' for Sum function");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGrandTotalName method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("MethodSetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


