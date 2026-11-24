---
title: "PivotField.ClearFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Löscht die Filtereinstellung dieses Pivot-Feldes"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/clearfilter/
---
## PivotField.ClearFilter method

Löscht die Filtereinstellung für dieses Pivot‑Feld.

```csharp
public void ClearFilter()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodClearFilterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Fruit";
            worksheet.Cells["A5"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["B5"].Value = 300;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hole das Pivot-Feld
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Wenden Sie zuerst einen Filter an, um das Löschen zu demonstrieren
                pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);

                // ClearFilter-Methode aufrufen
                pivotField.ClearFilter();

                Console.WriteLine("ClearFilter method executed successfully");
                Console.WriteLine("All filters have been removed from the pivot field");

                // Pivot-Tabelle aktualisieren, um Änderungen anzuzeigen
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


