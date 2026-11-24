---
title: "GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Namen der Feldüberschrift des Wertebereichs in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/
---
## GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable method

Gibt den Namen der Feldüberschrift des Wertebereichs in der PivotTable zurück.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfDataFieldHeader() method instead.")]
public virtual string GetDataFieldHeaderNameOfPivotTable()
```

### Rückgabewert

Der Name des Datenfeldüberschriftsnamens

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate nach Dezember 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 200;

            // Benutzerdefinierte Globalisierungseinstellungen festlegen
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // PivotTable erstellen und Felder konfigurieren
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B3", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category as row
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Value as data

                // PivotTable aktualisieren, um Lokalisierungsänderungen anzuwenden
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom data field header name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("GlobalizationSettingsMethodDemo.xlsx");
        }
    }

    // Benutzerdefinierte GlobalizationSettings-Implementierung
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDataFieldHeaderNameOfPivotTable()
        {
            return "Custom Values";
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


