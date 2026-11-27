---
title: "SettableGlobalizationSettings.GetGrandTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metod. Hämtar det totala summanamnet för funktionen"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/getgrandtotalname/
---
## SettableGlobalizationSettings.GetGrandTotalName method

Hämtar namnet på totalen för funktionen.

```csharp
public override string GetGrandTotalName(ConsolidationFunction functionType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | ConsolidationFunction | Funktionstypen. |

### Returvärde

Det totala namnet på funktionen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class SettableGlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ange anpassade totala summanamn för olika konsolideringsfunktioner
            settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Sum Grand Total");
            settings.SetGrandTotalName(ConsolidationFunction.Average, "Custom Average Grand Total");
            
            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Anropa GetGrandTotalName med olika konsolideringsfunktioner
                string sumGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Sum);
                string avgGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Average);
                
                // Skriv ut resultaten
                Console.WriteLine("Sum Grand Total Name: " + sumGrandTotalName);
                Console.WriteLine("Average Grand Total Name: " + avgGrandTotalName);

                // Skapa en pivottabell för att demonstrera effekten
                Cells cells = worksheet.Cells;
                cells["A1"].PutValue("Product");
                cells["B1"].PutValue("Sales");
                cells["A2"].PutValue("Apple");
                cells["B2"].PutValue(1000);
                cells["A3"].PutValue("Orange");
                cells["B3"].PutValue(2000);
                cells["A4"].PutValue("Banana");
                cells["B4"].PutValue(3000);

                PivotTableCollection pivotTables = worksheet.PivotTables;
                int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = pivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                
                // Korrekt sätt att lägga till ett annat datafält med Average-funktionen
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("SettableGlobalizationSettingsMethodGetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


