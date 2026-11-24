---
title: "GlobalizationSettings.GetGrandTotalName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Namen der Gesamtsumme der Funktion zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getgrandtotalname/
---
## GlobalizationSettings.GetGrandTotalName method

Gibt den Namen des Gesamtsummens der Funktion zurück.

```csharp
public virtual string GetGrandTotalName(ConsolidationFunction functionType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionType | ConsolidationFunction | Der Funktionstyp. |

### Rückgabewert

Der Gesamtsummenname der Funktion.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable füllen
            CreateSampleData(worksheet);

            // Instanziiere benutzerdefinierte Globalisierungseinstellungen
            var globalizationSettings = new CustomGlobalizationSettings();
            
            try
            {
                // Direkten Methodenaufruf demonstrieren
                string grandTotalName = globalizationSettings.GetGrandTotalName(ConsolidationFunction.Sum);
                Console.WriteLine($"Grand Total Name: {grandTotalName}");

                // Wende Anpassungen auf die Arbeitsmappeneinstellungen an
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Erstelle PivotTable, um die Wirkung zu demonstrieren
                CreatePivotTable(worksheet);

                Console.WriteLine("Method executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("GrandTotalNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Value";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Furniture";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Electronics";
            cells["B4"].Value = 800;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Erstelle PivotTable mit dem Beispiel-Datenbereich
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Konfiguriere PivotTable-Felder
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.Function = ConsolidationFunction.Sum;

            // Aktualisiere die Tabelle, um die Einstellungen anzuwenden
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetGrandTotalName(ConsolidationFunction functionType)
        {
            // Benutzerdefinierte Implementierung basierend auf Konsolidierungsfunktion
            return functionType == ConsolidationFunction.Sum 
                ? "**[Sum Total]**" 
                : base.GetGrandTotalName(functionType);
        }
    }
}
```

### Siehe auch

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


