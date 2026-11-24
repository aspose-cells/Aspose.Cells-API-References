---
title: "GlobalizationSettings.GetEmptyDataName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Namen des leeren Labels in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getemptydataname/
---
## GlobalizationSettings.GetEmptyDataName method

Gibt den Namen des "(blank)"-Labels in der PivotTable zurück.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfEmptyData() method instead.")]
public virtual string GetEmptyDataName()
```

### Rückgabewert

Der Name der leeren Daten

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate nach Dezember 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetEmptyDataNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten mit leeren Zellen
            object[,] data = new object[,]
            {
                {"Category", "Sales"},
                {"Electronics", 1500},
                {null, 2000}, // Empty category cell
                {"Furniture", 3000}
            };

            // Arbeitsblatt füllen
            int rows = data.GetLength(0);
            int cols = data.GetLength(1);
            for (int i = 0; i < rows; i++)
            {
                for (int j = 0; j < cols; j++)
                {
                    worksheet.Cells[i, j].PutValue(data[i, j]);
                }
            }

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            // Korrigiert: Ungültige Zuweisung des AddFieldToArea-Ergebnisses entfernen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Benutzerdefinierte Globalisierungseinstellungen konfigurieren
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Pivot-Tabelle aktualisieren, um die Lokalisierung anzuwenden
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Direkten Methodenaufruf demonstrieren
                string emptyName = workbook.Settings.GlobalizationSettings.GetEmptyDataName();
                Console.WriteLine($"Custom empty data label: {emptyName}");

                workbook.Save("GlobalizationGetEmptyDataNameDemo.xlsx");
                Console.WriteLine("Demo executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            [Obsolete]
            public override string GetEmptyDataName()
            {
                return "[[UNSPECIFIED]]"; // Custom empty data label
            }
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


