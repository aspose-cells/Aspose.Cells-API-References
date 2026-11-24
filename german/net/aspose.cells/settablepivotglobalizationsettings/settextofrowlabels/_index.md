---
title: "SettablePivotGlobalizationSettings.SetTextOfRowLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Legt den Text des Labels \"Row Labels\" in der PivotTable fest"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/settextofrowlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfRowLabels method

Setzt den Text des "Row Labels"-Labels in der PivotTable.

```csharp
public void SetTextOfRowLabels(string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Der Text der Zeilenbeschriftungen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Kontext hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Erstellen Sie Globalisierungseinstellungen
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            SettablePivotGlobalizationSettings pivotSettings = new SettablePivotGlobalizationSettings();
            globalizationSettings.PivotSettings = pivotSettings;

            try
            {
                // Benutzerdefinierten Text für "Row Labels" festlegen
                pivotSettings.SetTextOfRowLabels("Custom Row Labels");

                // Die Änderung überprüfen
                string rowLabelsText = pivotSettings.GetTextOfRowLabels();
                Console.WriteLine($"Row Labels text after change: {rowLabelsText}");

                // Einstellungen auf die Arbeitsmappe anwenden
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Speichere die Arbeitsmappe
                workbook.Save("SetTextOfRowLabelsDemo.xlsx");
                Console.WriteLine("SetTextOfRowLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


