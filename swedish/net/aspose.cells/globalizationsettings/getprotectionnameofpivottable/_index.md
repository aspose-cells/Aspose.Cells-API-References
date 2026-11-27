---
title: "GlobalizationSettings.GetProtectionNameOfPivotTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar skyddsnamnet i pivottabellen"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getprotectionnameofpivottable/
---
## GlobalizationSettings.GetProtectionNameOfPivotTable method

Hämtar skyddsnamnet i pivottabellen.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetProtectionNameOfPivotTable()
```

### Returvärde

Skyddsnamnet för pivottabellen

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetTextOfProtectedName(string). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa standardinställningar för globalisering
            GlobalizationSettings standardSettings = new GlobalizationSettings();
            
            // Skapa anpassade globaliseringsinställningar
            GlobalizationSettings customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Hämta standardskyddsnamn
                string defaultName = standardSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Default protection name: {defaultName}");

                // Hämta anpassat skyddsnamn
                string customName = customSettings.GetProtectionNameOfPivotTable();
                Console.WriteLine($"Custom protection name: {customName}");

                // Skapa pivottabell för att demonstrera tillämpning av inställningarna
                worksheet.Cells["A1"].Value = "Data";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;
                int pivotIndex = worksheet.PivotTables.Add("A1", "A1:A4", "PivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Skyddet skulle vanligtvis tillämpas här med det hämtade namnet
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetProtectionNameOfPivotTable: {ex.Message}");
            }
            
            workbook.Save("GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public new string GetProtectionNameOfPivotTable()
        {
            return "CustomPivotProtection";
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


