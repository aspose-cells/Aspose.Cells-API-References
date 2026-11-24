---
title: "GlobalizationSettings.GetMultipleItemsName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Namen des Labels „Multiple Items“ in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getmultipleitemsname/
---
## GlobalizationSettings.GetMultipleItemsName method

Gibt den Namen des Labels "(Multiple Items)" in der PivotTable zurück.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfMultipleItems() method instead.")]
public virtual string GetMultipleItemsName()
```

### Rückgabewert

Der Name des "(Multiple Items)"-Labels

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate nach Dezember 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetMultipleItemsNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für PivotTable vorbereiten
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // PivotTable erstellen
            int pivotIndex = worksheet.PivotTables.Add("D1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // PivotField konfigurieren, um mehrere Elemente anzuzeigen
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.HideItem(0, false); // Select "A"
            rowField.HideItem(1, false); // Select "B"

            // Globalisierungseinstellungen initialisieren
            GlobalizationSettings gSettings = workbook.Settings.GlobalizationSettings ?? new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings = gSettings;

            try
            {
                // Rufe GetMultipleItemsName auf und zeige das Ergebnis an
                string multipleItemsName = gSettings.GetMultipleItemsName();
                Console.WriteLine($"Multiple Items Name: {multipleItemsName}");

                // PivotTable aktualisieren, um die Einstellungen anzuwenden
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetMultipleItemsName: {ex.Message}");
            }

            // Arbeitsmappe speichern, um die PivotTable mit dem Label für mehrere Elemente anzuzeigen
            workbook.Save("GlobalizationSettingsMethodGetMultipleItemsNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


