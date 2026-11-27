---
title: "GlobalizationSettings.GetTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar totalnamnet för funktionen"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/gettotalname/
---
## GlobalizationSettings.GetTotalName method

Hämtar totalnamnet för funktionen.

```csharp
public virtual string GetTotalName(ConsolidationFunction functionType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | ConsolidationFunction | Funktionstypen. |

### Returvärde

Totalnamnet för funktionen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;

            // Skapa anpassade globaliseringsinställningar
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Demonstrera direkt metodanrop
                Console.WriteLine("Sum Total Name: " + 
                    customSettings.GetTotalName(ConsolidationFunction.Sum));
                
                // Skapa pivottabell för att utlösa användning av GetTotalName
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;

                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom total names");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTotalName(ConsolidationFunction functionType)
            {
                return functionType switch
                {
                    ConsolidationFunction.Sum => "[Sum Custom]",
                    ConsolidationFunction.Count => "[Count Custom]",
                    _ => base.GetTotalName(functionType)
                };
            }
        }
    }
}
```

### Se även

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


