---
title: "PivotFieldSortSetting.FieldIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFieldSortSetting-Eigenschaft. Gibt den Index des sortierten Feldes an. 1 bedeutet, dass das PivotField nach den Beschriftungen sortiert wird, andere Werte bedeuten, dass nach dem Datenfeld sortiert wird."
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldsortsetting/fieldindex/
---
## PivotFieldSortSetting.FieldIndex property

Gibt den Index des sortierten Feldes an. -1 bedeutet, dass das PivotField nach den Beschriftungen sortiert wird, andere Werte bedeuten, dass nach dem Datenfeld sortiert wird.

```csharp
[Obsolete("Use PivotFieldSortSetting.SortBy property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int FieldIndex { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die PivotFieldSortSetting.SortBy‑Eigenschaft. Diese Methode wird 12 Monate nach September 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // PivotField‑Sortiereinstellung abrufen
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;

            // Aktuellen FieldIndex‑Wert anzeigen
            Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);

            // Hinweis: FieldIndex ist schreibgeschützt und PivotFieldSortSetting kann nicht direkt instanziiert werden
            // da es keinen öffentlichen Konstruktor hat. Wir können nur mit der bestehenden Instanz arbeiten
            // erhalten aus der SortSetting‑Eigenschaft des PivotFields.

            // Aktualisieren Sie die Pivot-Tabelle, um Änderungen anzuwenden
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ergebnis speichern
            workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


