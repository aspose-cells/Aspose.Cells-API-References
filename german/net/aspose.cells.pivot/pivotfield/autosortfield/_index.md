---
title: "PivotField.AutoSortField"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField‑Eigenschaft. Gibt den Index des Feldes an, das automatisch sortiert wird. 1 bedeutet das PivotField selbst, andere Werte bedeuten die Position der Datenfelder."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Gibt den Index des Feldes an, das automatisch sortiert wird. -1 bedeutet das PivotField selbst, andere Werte bedeuten die Position der Datenfelder.

```csharp
[Obsolete("Use PivotField.SortSetting.SortBy property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoSortField { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die PivotField.SortSetting.SortBy‑Eigenschaft oder die PivotField.SortBy()‑Methode. Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoSortFieldDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Branch";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "North";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "South";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "East";
            cells["B4"].Value = 800;
            cells["A5"].Value = "West";
            cells["B5"].Value = 1200;

            // PivotTable hinzufügen
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hole das Pivot-Feld
            PivotField pivotField = pivotTable.RowFields["Branch"];

            // Automatisches Sortieren konfigurieren
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.AutoSortField = 0; // Sort by first data field (Sales)

            // Berechne Daten und aktualisiere
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldAutoSortDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


