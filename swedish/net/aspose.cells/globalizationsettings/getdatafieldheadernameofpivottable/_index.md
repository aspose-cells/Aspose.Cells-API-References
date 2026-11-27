---
title: "GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar namnet på fältets rubrik för värdeområdet i PivotTable"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/
---
## GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable method

Hämtar namnet på fältets rubrik för värdeområdet i PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfDataFieldHeader() method instead.")]
public virtual string GetDataFieldHeaderNameOfPivotTable()
```

### Returvärde

Namnet på datafältets rubrik

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetColumnLabelsOfPivotTable()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetDataFieldHeaderNameOfPivotTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för PivotTable
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 200;

            // Ställ in anpassade globaliseringsinställningar
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Skapa PivotTable och konfigurera fält
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B3", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category as row
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Value as data

                // Uppdatera PivotTable för att tillämpa lokaliseringsändringar
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom data field header name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("GlobalizationSettingsMethodDemo.xlsx");
        }
    }

    // Anpassad GlobalizationSettings-implementation
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDataFieldHeaderNameOfPivotTable()
        {
            return "Custom Values";
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


