---
title: "GlobalizationSettings.GetEmptyDataName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar namnet på den tomma etiketten i pivottabellen"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getemptydataname/
---
## GlobalizationSettings.GetEmptyDataName method

Hämtar namnet på "(blank)"-etiketten i pivottabellen.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfEmptyData() method instead.")]
public virtual string GetEmptyDataName()
```

### Returvärde

Namnet på tomma data

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetColumnLabelsOfPivotTable()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetEmptyDataNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata med tomma celler
            object[,] data = new object[,]
            {
                {"Category", "Sales"},
                {"Electronics", 1500},
                {null, 2000}, // Empty category cell
                {"Furniture", 3000}
            };

            // Fyll i kalkylbladet
            int rows = data.GetLength(0);
            int cols = data.GetLength(1);
            for (int i = 0; i < rows; i++)
            {
                for (int j = 0; j < cols; j++)
                {
                    worksheet.Cells[i, j].PutValue(data[i, j]);
                }
            }

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            // Korrigerat: Ta bort ogiltig tilldelning av resultatet från AddFieldToArea
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Konfigurera anpassade globaliseringsinställningar
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Uppdatera pivottabellen för att tillämpa lokalisering
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Demonstrera direkt metodanrop
                string emptyName = workbook.Settings.GlobalizationSettings.GetEmptyDataName();
                Console.WriteLine($"Custom empty data label: {emptyName}");

                workbook.Save("GlobalizationGetEmptyDataNameDemo.xlsx");
                Console.WriteLine("Demo executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            [Obsolete]
            public override string GetEmptyDataName()
            {
                return "[[UNSPECIFIED]]"; // Custom empty data label
            }
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


