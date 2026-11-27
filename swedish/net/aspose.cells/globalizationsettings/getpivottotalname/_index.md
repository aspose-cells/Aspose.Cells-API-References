---
title: "GlobalizationSettings.GetPivotTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar namnet på Total-etiketten i PivotTable. Du måste åsidosätta denna metod när PivotTable innehåller två eller fler PivotFields i dataområdet."
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getpivottotalname/
---
## GlobalizationSettings.GetPivotTotalName method

Hämtar namnet på "Total"-etiketten i PivotTable. Du måste åsidosätta denna metod när PivotTable innehåller två eller fler PivotFields i dataområdet.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotTotalName()
```

### Returvärde

Namnet på "Total"-etiketten

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetColumnLabelsOfPivotTable()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotTotalNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "North"; worksheet.Cells["B2"].Value = 1000; worksheet.Cells["C2"].Value = 50;
            worksheet.Cells["A3"].Value = "South"; worksheet.Cells["B3"].Value = 2000; worksheet.Cells["C3"].Value = 70;
            worksheet.Cells["A4"].Value = "West"; worksheet.Cells["B4"].Value = 3000; worksheet.Cells["C4"].Value = 110;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E5", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Quantity

            // Skapa och konfigurera globaliseringsinställningar
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Demonstrera direkt metodanrop
                Console.WriteLine("Custom Total Name: " + customSettings.GetPivotTotalName());

                // Bearbeta pivottabell
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Pivot table created with custom total name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetPivotTotalNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetPivotTotalName()
        {
            return "Custom Total";
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


