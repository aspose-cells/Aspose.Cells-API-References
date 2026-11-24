---
title: "GlobalizationSettings.GetAllName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Namen des All‑Labels in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getallname/
---
## GlobalizationSettings.GetAllName method

Gibt den Namen des \"(All)\"-Labels in der PivotTable zurück.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfAll() method instead.")]
public virtual string GetAllName()
```

### Rückgabewert

Der Name des \"(All)\"-Labels

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode GlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetAllNameDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit benutzerdefinierten Globalisierungseinstellungen
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Greifen Sie auf die Instanz der benutzerdefinierten Einstellungen zu
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            try
            {
                // Rufen Sie die GetAllName-Methode auf und zeigen Sie das Ergebnis an
                string allName = settings.GetAllName();
                Console.WriteLine($"Custom (All) label: {allName}");

                // Erstellen Sie eine Beispiel-PivotTable, um die Lokalisierungswirkung zu demonstrieren
                Worksheet worksheet = workbook.Worksheets[0];
                CreateSampleData(worksheet);
                CreatePivotTable(worksheet);

                Console.WriteLine("Demo executed successfully. Check output file's pivot table labels.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("MethodGetAllNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Beispieldaten für Pivot‑Tabelle erstellen
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Cars";
            worksheet.Cells["A4"].Value = "Bikes";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["B4"].Value = 1500;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Erstellen Sie eine PivotTable mit Beispieldaten
            int pivotIndex = worksheet.PivotTables.Add(
                "PivotTable",
                "A1:B4",
                "E3"
            );
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Konfigurieren Sie die Struktur der PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields[0]); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[1]); // Sales

            // Aktualisieren Sie die Tabelle, um die Lokalisierungseinstellungen anzuwenden
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetAllName()
        {
            // Benutzerdefinierte Implementierung gibt das lokalisierte \"All\"-Label zurück
            return "[Custom All Selection]";
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


