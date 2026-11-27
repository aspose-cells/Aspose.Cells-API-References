---
title: "GlobalizationSettings.GetRowLabelsNameOfPivotTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar namnet på Row Labels-etiketten i PivotTable"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/
---
## GlobalizationSettings.GetRowLabelsNameOfPivotTable method

Hämtar namnet på "Row Labels"-etiketten i PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfRowLabels() method instead.")]
public virtual string GetRowLabelsNameOfPivotTable()
```

### Returvärde

Namnet på radetiketter

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetColumnLabelsOfPivotTable()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetRowLabelsNameOfPivotTable()
        {
            return "Custom Row Labels";
        }
    }

    public class GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["A2"].PutValue("Bikes");
            cells["A3"].PutValue("Cars");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(1000);
            cells["B3"].PutValue(2500);

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B3", "E3", "SalesPivot");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field

            // Tillämpa anpassade globaliseringsinställningar
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                Console.WriteLine("Pivot table created with custom row labels name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowLabelsNameOfPivotTable: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo.xlsx");
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


