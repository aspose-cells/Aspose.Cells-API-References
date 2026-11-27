---
title: "GlobalizationSettings.GetGrandTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar namnet på den totala summan för funktionen"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getgrandtotalname/
---
## GlobalizationSettings.GetGrandTotalName method

Hämtar namnet på totalen för funktionen.

```csharp
public virtual string GetGrandTotalName(ConsolidationFunction functionType)
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
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata för pivottabellen
            CreateSampleData(worksheet);

            // Instansiera anpassade globaliseringsinställningar
            var globalizationSettings = new CustomGlobalizationSettings();
            
            try
            {
                // Demonstrera direkt metodanrop
                string grandTotalName = globalizationSettings.GetGrandTotalName(ConsolidationFunction.Sum);
                Console.WriteLine($"Grand Total Name: {grandTotalName}");

                // Tillämpa anpassning på arbetsbokinställningarna
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Skapa pivottabell för att demonstrera effekten
                CreatePivotTable(worksheet);

                Console.WriteLine("Method executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("GrandTotalNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Value";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Furniture";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Electronics";
            cells["B4"].Value = 800;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Skapa pivottabell med hjälp av exempeldataområde
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Konfigurera pivottabellens fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.Function = ConsolidationFunction.Sum;

            // Uppdatera tabellen för att tillämpa inställningarna
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetGrandTotalName(ConsolidationFunction functionType)
        {
            // Anpassad implementation baserad på konsolideringsfunktion
            return functionType == ConsolidationFunction.Sum 
                ? "**[Sum Total]**" 
                : base.GetGrandTotalName(functionType);
        }
    }
}
```

### Se även

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


