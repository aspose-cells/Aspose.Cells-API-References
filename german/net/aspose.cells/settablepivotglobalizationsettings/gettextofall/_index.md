---
title: "SettablePivotGlobalizationSettings.GetTextOfAll"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Gibt den Text der \"All\"‑Beschriftung in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/gettextofall/
---
## SettablePivotGlobalizationSettings.GetTextOfAll method

Ermittelt den Text der Beschriftung "(All)" in der PivotTable.

```csharp
public override string GetTextOfAll()
```

### Rückgabewert

Der Text der "(All)"‑Beschriftung

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfAllDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(15);

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Erstellen Sie Globalisierungseinstellungen
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();
            settings.SetTextOfAll("(All Items)");

            try
            {
                // Rufen Sie den aktuellen Text der "(All)"‑Beschriftung ab
                string currentText = settings.GetTextOfAll();
                Console.WriteLine($"Current text of '(All)' label: {currentText}");

                // PivotTable mit neuen Einstellungen aktualisieren
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfAll method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("MethodGetTextOfAllDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


