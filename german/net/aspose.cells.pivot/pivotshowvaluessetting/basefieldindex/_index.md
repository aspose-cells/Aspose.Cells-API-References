---
title: "PivotShowValuesSetting.BaseFieldIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotShowValuesSetting-Eigenschaft. Repräsentiert das Basisfeld für eine ShowDataAs-Berechnung, wenn die ShowDataAs-Berechnung verwendet wird"
type: docs
url: /de/net/aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/
---
## PivotShowValuesSetting.BaseFieldIndex property

Stellt das Basisfeld für eine ShowDataAs‑Berechnung dar, wenn die ShowDataAs‑Berechnung verwendet wird.

```csharp
public int BaseFieldIndex { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingPropertyBaseFieldIndexDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            try
            {
                // Pivot-Tabelle erstellen
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Felder zur Pivot-Tabelle hinzufügen
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Abrufen des Datenfelds und seiner Anzeigeeinstellung für Werte
                PivotField dataField = pivotTable.DataFields[0];
                PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

                // Berechnungstyp festlegen, um die Verwendung von BaseFieldIndex zu demonstrieren
                showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;

                // BaseFieldIndex-Eigenschaft festlegen und abrufen
                showValuesSetting.BaseFieldIndex = 0;
                Console.WriteLine("BaseFieldIndex value: " + showValuesSetting.BaseFieldIndex);

                // Pivot-Tabelle aktualisieren und berechnen
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Speichere die Arbeitsmappe
                workbook.Save("BaseFieldIndexDemo.xlsx");
                Console.WriteLine("BaseFieldIndex has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


