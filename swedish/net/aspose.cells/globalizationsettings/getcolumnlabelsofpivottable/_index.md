---
title: "GlobalizationSettings.GetColumnLabelsOfPivotTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings metod. Hämtar namnet på etiketten \\\"Column Labels\\\" i pivottabellen."
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/
---
## GlobalizationSettings.GetColumnLabelsOfPivotTable method

Hämtar namnet på etiketten \"Column Labels\" i pivottabellen.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfColumnLabels() method instead.")]
public virtual string GetColumnLabelsOfPivotTable()
```

### Returvärde

Namnet på kolumnetiketter

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetColumnLabelsOfPivotTable()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetColumnLabelsOfPivotTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 10000;
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 8000;
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 25000;

            // Skapa en pivottabell och hämta referens
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C4", "E5");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Tillämpa anpassade globaliseringsinställningar för att åsidosätta kolumnetiketter
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Uppdatera och beräkna pivottabellen för att tillämpa inställningarna
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetColumnLabelsOfPivotTable method executed successfully. Check 'output.xlsx'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }

    // Anpassad GlobalizationSettings‑implementation för att åsidosätta kolumnetiketter
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetColumnLabelsOfPivotTable()
        {
            // Returnera anpassad etikett för pivottabellens kolumnrubriker
            return "Sales Regions";
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


