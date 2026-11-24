---
title: "GlobalizationSettings.GetColumnLabelsOfPivotTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings‑Methode. Gibt den Namen des Spaltenbeschriftungs‑Labels in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/
---
## GlobalizationSettings.GetColumnLabelsOfPivotTable method

Gibt den Namen des "Column Labels"‑Labels in der PivotTable zurück.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfColumnLabels() method instead.")]
public virtual string GetColumnLabelsOfPivotTable()
```

### Rückgabewert

Der Name der Spaltenbeschriftungen

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate nach Dezember 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable füllen
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

            // Erstellen Sie eine PivotTable und erhalten Sie eine Referenz
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C4", "E5");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Wenden Sie benutzerdefinierte Globalisierungseinstellungen an, um Spaltenbeschriftungen zu überschreiben
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Aktualisieren und berechnen Sie die PivotTable, um die Einstellungen anzuwenden
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetColumnLabelsOfPivotTable method executed successfully. Check 'output.xlsx'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }

    // Benutzerdefinierte GlobalizationSettings-Implementierung zum Überschreiben von Spaltenbeschriftungen
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetColumnLabelsOfPivotTable()
        {
            // Gibt ein benutzerdefiniertes Label für die Spaltenüberschriften der PivotTable zurück
            return "Sales Regions";
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


